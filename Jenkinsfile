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
                    
                    
            }
        }
        stage('two'){
           steps{
               bat 'mkdir C:\\test'
           }
       }
        stage('three') {
            
            steps {
                bat 'echo hello! I am William > C:\\test\\sample.txt'
            }
        }
        stage('mail'){
            steps{
                mail bcc: '',attachmentsPattern: 'C:\\test\\sample.txt', body: "<br>\n<br>Project: ${env.JOB_NAME} <br>Build Number: ${env.BUILD_NUMBER} <br> URL build: ${env.BUILD_URL}", from: '', replyTo: '',subject: 'Demo Mail', to: 'William.Carey@analog.com';
       }
    }
}
}
