pipeline{
    agent any
    environment{
        BRANCH_NAME = "${GIT_BRANCH.split("/")[1]}"
    }
   
    stages{
         
        stage('one'){
            steps{
                    
                    cleanWs()
                    echo "${BRANCH_NAME}"
                bat 'mkdir Hello'
                    
                    
            }
        }
        stage('two'){
            steps{
                bat 'cd Hello'
            }
        }
    }
}
