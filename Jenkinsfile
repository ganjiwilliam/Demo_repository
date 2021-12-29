u
pipeline{
    agent any
	environment{	        
		ENV_NAME = "${GIT_BRANCH.split("/")[1] == "feature" ? "${GIT_BRANCH.split("/")[0]}" : "no"}"
	}
    stages{         
        stage('one'){
            steps{                    
                    cleanWs()
		    echo "${ENV_NAME}"
                                                   
	        }    
            }
        }
  
}
