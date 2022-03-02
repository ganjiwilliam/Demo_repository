pipeline{
    agent any
    environment{
        
        BRANCH_NAME = "${GIT_BRANCH.split("/")[1] == "development" ? "development" : GIT_BRANCH.split("/")[1] == "release" ? "${GIT_BRANCH.split("/")[2]}" : "${GIT_BRANCH.split("/")[2].substring(0, 24)}"}"
    }
    stages{
        stage('macro'){
            steps{
                bat '''
               echo %BRANCH_NAME%
                '''
            }
        }
    }
}
