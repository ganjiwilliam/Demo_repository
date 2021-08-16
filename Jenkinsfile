pipeline {
         agent any
         environment{
                   a='jenkins'
         }
         stages {
                 stage('One') {
                 steps {
                          script{
                             bat 'echo %GIT_URL% >> git.txt'
                             bat 'echo %GIT_COMMIT% >> git.txt'
                             bat 'echo %GIT_BRANCH% >> git.txt'
                             a=a[1..4]
                             bat 'echo %a% >> git.txt' 
                             
                             
                          }
              
                 }
                 }
         }      
}
