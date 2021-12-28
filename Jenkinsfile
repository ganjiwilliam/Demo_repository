
pipeline{
    agent any
	environment{
		ENV_NAME = "${GIT_BRANCH == "main" ? "staging" : "production"}"
    stages{         
        stage('one'){
            steps{                    
                    cleanWs()
		    echo "${ENV_NAME}"
                                                   
	        }    
            }
        }
  
}
