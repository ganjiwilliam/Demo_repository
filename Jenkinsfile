pipeline {
         agent any
         environment{
        BRANCH_NAME = "${GIT_BRANCH}"
    }
         stages {
                 stage('One') {
                 steps {
                          ws('C:\\yoyo'){ 
                          echo "hello william"
                          bat '''mkdir adiPeopleCount-CM-Rel%BRANCH_NAME%_PROD '''
                          }
                          }
                 }
                 
         }      
}
