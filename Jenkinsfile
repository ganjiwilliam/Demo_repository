pipeline {
         agent any
         
         stages {
                 stage('One') {
                 steps {
                          script{
                             
                             bat 'echo %GIT_BRANCH% >> git.txt'
                             set a= %GIT_BRANCH%
                             a=a[15..19]       
                                   
                          }
              
                 }
                 }
         }      
}
