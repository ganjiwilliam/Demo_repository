pipeline {
         agent any
         stages {
                 stage('One') {
                 steps {
                    
                        
                             bat 'echo %GIT_URL% >> git.txt'
                             bat 'echo %GIT_COMMIT% >> git.txt'
                              bat 'echo %GIT_BRANCH% >> git.txt'
                          bat '''set OutputFolderName=%date:~12,2%%date:~4,2%%date:~7,2%_%time:~0,2%%time:~3,2%%time:~6,2%release/3.4.0
                          mkdir %OutputFolderName% '''
                        
                          
                 }
                 }
         }      
}
