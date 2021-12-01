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
           mail bcc: '', body: "<b>Example</b><br>\n\<br>Project: ${env.JOB_NAME} <br>Build Number: ${env.BUILD_NUMBER} <br> URL build: ${env.BUILD_URL}", cc: '', charset: 'UTF-8', from: 'nnn', mimeType: 'text/html', replyTo: 'ganjiwilliam@gmail.com', subject: "ERROR CI: Project name -> ${env.JOB_NAME}", to: "foo@foomail.com";
        }
    }
}
