
pipeline{
    agent any
	environment{
		ENV_NAME = "${GIT_BRANCH.split("/")[1] == "main" ? "staging" : "production"}"
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
