pipeline {
         agent any
         environment{
                  a= %GIT_BRANCH%
         }
         stages {
                 stage('One') {
                 steps {
                          script{
                             bat 'echo %GIT_URL% >> git.txt'
                             bat 'echo %GIT_COMMIT% >> git.txt'
                             bat 'echo %GIT_BRANCH% >> git.txt'
                             
                             bat '''set OutputFolderName=%GIT_COMMIT%
                             mkdir %OutputFolderName% '''
                          }
              
                 }
                 }
         }      
}
