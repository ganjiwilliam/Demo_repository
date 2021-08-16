pipeline {
         agent any
         environment{
                  a="williamcarey"
         stages {
                 stage('One') {
                 steps {
                          
                             
                             bat 'echo %GIT_BRANCH% >> git.txt'
                             a=a[7..11]
                          bat 'echo ${a}' 
                       
                 }
                 }
         }      
}
