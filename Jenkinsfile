
pipeline{
    agent any
	environment{
		BRANCH_NAME="${GIT_BRANCH.split("/")[1]}"
		if ${BRANCH_NAME}==main (echo "hello")
    stages{         
        stage('one'){
            steps{                    
                    cleanWs()
		    echo "${BRANCH_NAME}"
                                                   
	        }    
            }
        }
  
}
