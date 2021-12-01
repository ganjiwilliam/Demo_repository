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
        stage('mail'){
            steps{
                mail bcc: '', body: "<br>\n<br>Project: ${env.JOB_NAME} <br>Build Number: ${env.BUILD_NUMBER} <br> URL build: ${env.BUILD_URL}", from: '', replyTo: '',subject: 'Demo Mail', to: 'William.Carey@analog.com';
    }
    post {
        always {
           
        }
    }
}
