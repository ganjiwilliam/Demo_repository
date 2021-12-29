
pipeline{
    agent any
	environment{	        
		RELEASE_NUM = "${GIT_BRANCH.split("/")[1] == "feature" ? "${GIT_BRANCH.split("/")[2]~0,10}" : "${GIT_BRANCH.split("/")[2]}"}"
	}
    stages{         
        stage('one'){
            steps{                    
                    cleanWs()
		    echo "${RELEASE_NUME}"
                                                   
	        }    
            }
        }
  
}
