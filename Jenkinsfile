
def call{
	BRANCH_NAME = "${GIT_BRANCH.split("/")[1]}"
	
pipeline{
    agent any

    
    stages{         
        stage('one'){
            steps{                    
                    cleanWs()
		    echo "${BRANCH_NAME}"
                                                   
	        }    
            }
        }
}   
}
