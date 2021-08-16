pipeline {
         agent any
         
         stages {
                 stage('One') {
                 steps {
                          script{
                             bat 'echo %GIT_URL% >> git.txt'
                             bat 'echo %GIT_COMMIT% >> git.txt'
                             bat 'echo %GIT_BRANCH% >> git.txt'
                             set a=%GIT_BRANCH%[15..19]
                          }
              
                 }
                 }
         }      
}
