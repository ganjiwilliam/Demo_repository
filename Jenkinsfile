pipeline{
    agent any
    stages{
        stage('one'){
            steps{
                dir('C:\\willgitdir'){
                    bat ''' 
                     echo %GIT_URL% >>  ..\\svn.txt
                    '''
                }
            }
        }
    }
}
