pipeline {
         agent any
         environment{
        BRANCH_NAME = "${GIT_BRANCH}"
    }
         stages {
                 stage('One') {
                 steps {
                          ws('C:\\yoyo'){ 
                         bat '''
                         echo echo %BRANCH_NAME% >>  ..\\svn.txt
                          '''
                          }
                          }
                 }
                 
         }      
}
