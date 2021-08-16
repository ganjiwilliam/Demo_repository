pipeline {
         agent any
         stages {
                 stage('One') {
                 steps {
                     echo 'Hi, this is william'
                 }
                 }
                  stage('Two'){
                           script{
                                    GIT_SHORT_COMMIT = sh(returnStdout: true, script: "git log -n 1 --pretty=format:'%h'").trim()
                                    echo GIT_SHORT_COMMIT
         
         
         }      
}
