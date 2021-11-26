pipeline {
         agent any
         environment{
        BRANCH_NAME = "${GIT_BRANCH}"
    }
         stages {
                 stage('One') {
                 steps {
                          ws('C:\\demoo'){ 
                         bat '''
                          echo %BRANCH_NAME% >>  ..\\svn.txt
                          '''
                          }
                          }
                 }
                 
         }      
}
