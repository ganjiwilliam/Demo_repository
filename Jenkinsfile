pipeline {
         agent any
         environment{
                  a="williamcarey"
         }
         stages {
                 stage('One') {
                          steps { 
                                   script{
                             bat 'echo %GIT_BRANCH% >> git.txt'
                             a=a[7..11]
                             echo "${a}"
                                            bat 'echo ${a}'
                             
                                   }
                       
                 }
                 }
         }      
}
