pipeline {
         agent any
         
         stages {
                 stage('One') {
                 steps {
                          script{
                             
                             bat 'echo %GIT_BRANCH% >> git.txt'
                                   
                          }
              
                 }
                 }
         }      
}
