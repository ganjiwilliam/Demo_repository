
pipeline{
    agent any
	environment{	        
		ENV_NAME = "${GIT_BRANCH.split("/")[1] == "main" ? "${GIT_BRANCH.split("/")[0]}" : "no"}"
	}
    stages{         
        stage('one'){
            steps{     
		    bat 'mkdir hello1'
                    cleanWs()
		    echo "${ENV_NAME}"
		    bat 'mkdir hello2'
                                                   
	        }    
            }
        }
  
}
