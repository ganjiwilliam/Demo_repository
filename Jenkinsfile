pipeline {
         agent any
         
         stages {
                 stage('One') {
                 steps {
                          ws('D:\\Jenkins\\xyz'){
                        
                             bat ''' echo %GIT_URL% >> git.txt
                                     echo %GIT_COMMIT% >> git.txt
                                     echo %GIT_BRANCH% >> git.txt
                                      '''
                          }
                 }
                 }
         }      
}
