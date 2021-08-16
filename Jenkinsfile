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
                             
                             set var1=A
                             set var2=B
                             set AB=hi
                             set newvar=!%var1%%var2%!
                             echo %newvar%
                             
                             
                          }
              
                 }
                 }
         }      
}
