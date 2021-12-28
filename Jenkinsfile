
pipeline{
    agent any
	environment{
		ENV_NAME = "${GIT_BRANCH.split("/")[1] == "main" ? "GIT_BRANCH.split("/")[1] : "GIT_BRANCH.split("/")[1]"}
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
