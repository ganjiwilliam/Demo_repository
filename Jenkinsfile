pipeline{
    agent any
    stages{
        stage('one'){
            steps{
                dir('C:\\willgitdir'){
                     
                     checkout([$class: 'GitSCM', branches: [[name: '*/main']], extensions: [[$class: 'CloneOption', timeout: 120]], userRemoteConfigs: [[credentialsId: '6322c427-7af4-439f-b2a2-d20f8313a5ad', url: 'https://github.com/ganjiwilliam/Demo_repository.git']]])
                     echo "${GIT_BRANCH}"
                   
                }
            }
        }
    }
}
