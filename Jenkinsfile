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
                             echo "${a.substring()}"
                             bat '''setlocal EnableDelayedExpansion
                             set var1=A
                             set var2=B
                             set AB=hi
                              set newvar=!%var1%%var2%!
                               echo %newvar% ''' 
                                   }
                       
                 }
                 }
         }      
}
