pipeline {
         agent any
         environment{
        BRANCH_NAME = "${GIT_BRANCH.split("/")[2]}"
    }
         stages {
                 stage('One') {
                 steps {
                          
                          echo "hello william"
                          bat '''mkdir adiPeopleCount-CM-Rel%BRANCH_NAME%_PROD '''
                          }
                 }
                 
         }      
}
