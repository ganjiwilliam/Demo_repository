pipeline {
         agent any
         
         stages {
                 stage('One') {
                 steps {
                          
                             
                             bat 'echo %GIT_BRANCH% >> git.txt'
                             bat '''set a= %GIT_BRANCH%
                           a=a[15..19]
                           echo %a% >> git.txt'''    
                                   
                          
              
                 }
                 }
         }      
}
