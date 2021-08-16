pipeline {
         agent any
         environment{
     BRANCH_NAME = "${GIT_BRANCH.split("/")[1]}"
  }


         }
         stages {
                 stage('One') {
                          steps { 
                                   script{
                             bat 'echo %GIT_BRANCH% >> git.txt'
                                            echo "${BRAnCH_NAME}"
                                           
                                            }
                             
                                   }
                       
                 }
                 }
         }      
}
