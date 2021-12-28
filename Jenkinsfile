pipeline{
    agent any
    environment{
        BRANCH_NAME = "${GIT_BRANCH.split("/")[1]}"
    }
   
    stages{
         
        stage('one'){
            steps{
                    
                    cleanWs()
		    echo "${GIT_BRANCH}"
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
    post{
        always{
            emailext (attachLog: true,compressLog: true,
		            body: """Job Name : ${env.JOB_NAME}
                    Build Number : $BUILD_NUMBER
                    Status : ${currentBuild.result}
                    URL to Jenkins Build : ${env.BUILD_URL}""",
                    subject: 'automation reports', to: 'William.Carey@analog.com')
        }
    }
}
