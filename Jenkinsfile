pipeline{
    agent any
    environment{
        BRANCH_NAME = "${GIT_BRANCH.split("/")[2]}"
    }
    stages{
        stage('one'){
            steps{
                bat 'echo %GIT_BRANCH% >> git.txt'
                echo "${BRANCH_NAME}"
                bat 'echo %BRAnCH_NAME%'
                bat ' ren "adiEagleEye_PeopleCount_Signed_Encrypted_App_v.ldr" "adiEagleEye_PeopleCount_Signed_Encrypted_App_v%BRAnCH_NAME%.ldr" '
                    
                }
            }
        
    }
}
