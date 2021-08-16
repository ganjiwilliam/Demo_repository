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
                                      echo "${BRANCH_NAME}"
                                      bat 'echo %BRAnCH_NAME%'
                                      bat ' ren "git.txt" "git%BRAnCH_NAME%.txt" '
                                      
                                      
                                   }
                            }
                 }
                 
         }      
}
