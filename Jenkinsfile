
pipeline{
    agent any
	environment{	        
		ENV_NAME = "${GIT_BRANCH.split("/")[1] == "main" ? "yes" : "no"}
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
