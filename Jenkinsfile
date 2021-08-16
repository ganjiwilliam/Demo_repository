pipeline {
         agent any
         environment{
                  a= "williamcarey"
         }
         stages {
                 stage('One') {
                          steps { 
                                   script{
                             bat 'echo %GIT_BRANCH% >> git.txt'
                             a=a[7..11]
                             echo "${a}"
                                            withEnv(["x=${GIT_BRANCH}"]){
                                                     x=x[15..19]
                                      bat 'echo %x%'
                                            }
                             
                                   }
                       
                 }
                 }
         }      
}
