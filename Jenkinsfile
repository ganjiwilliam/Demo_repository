pipeline{
    agent any
    environment{
        BRANCH_NAME = "${GIT_BRANCH.split("/")[1]}"
    }
    stages{
        stage('one'){
            steps{
               
                dir('C:\\willgitdir'){
                     cleanWs()
                                          echo "${BRANCH_NAME}"
                    bat 'mkdir hey'
                    bat 'del README.md'
                }
            }
        }
    }
}
