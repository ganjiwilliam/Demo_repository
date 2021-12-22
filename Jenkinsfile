pipeline{
    agent any
    environment{
        BRANCH_NAME = "${GIT_BRANCH.split("/")[1]}"
    }
    ws('C:\\mydemo'){
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
