
pipeline{
    agent any
	environment{	        
		ENV_NAME = "${GIT_BRANCH.split("/")[1] == "feature" ? "${GIT_BRANCH.split("/")[2]:0:10}" : "${GIT_BRANCH.split("/")[2]}"}"
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
