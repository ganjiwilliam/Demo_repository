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
                    bat 'mkdir hey'
                    bat 'del README.md'
            }
        }
    }
    post {
        always {
           mail  body: "Project: ${env.JOB_NAME} <br>Build Number: ${env.BUILD_NUMBER} <br> URL build: ${env.BUILD_URL}";
        }
    }
}
