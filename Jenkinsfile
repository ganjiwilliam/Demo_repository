pipeline {
         agent any
         environment{
     BRANCH_NAME = "${GIT_BRANCH.split("/")[2]}"
  }
         stages {
                 stage('One') {
                          steps { 
                                   script{
                                      bat 'echo %GIT_BRANCH% >> git.txt'
                                      bat 'echo %BRAnCH_NAME%'
                                      
                                   }
                            }
                 }
                 
         }      
}
