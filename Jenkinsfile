pipeline{
    agent any
    environment{
        BRANCH_NAME = "${GIT_BRANCH.split("/")[1]}"
    }
   
    stages{
         ws('C:\\mydemo'){
        stage('one'){
            steps{
                    cleanWs()
                    echo "${BRANCH_NAME}"
                    
                    
            }
        }
    }
    }
}
