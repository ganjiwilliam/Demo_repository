pipeline {
         agent any
         stages {
                 stage('One') {
                 steps {
                     def a=checkout([$class: 'GitSCM', branches: [[name: '*/main']], extensions: [], userRemoteConfigs: [[credentialsId: 'c54bedfe-f1ce-4740-af7d-42900c2a17f3', url: 'https://github.com/ganjiwilliam/Demo_repository.git']]])
                     withEnv(["GIT_URL=${a.GIT_URL}","GIT_COMMIT=${a.GIT_COMMIT}","GIT_BRANCH=${a.GIT_BRANCH}"]){
                        
                             bat 'echo %GIT_URL% >> git.txt'
                             bat 'echo %GIT_COMMIT% >> git.txt'
                              bat 'echo %GIT_BRANCH% >> git.txt'
                        }
                          echo 'Hi, this is william'
                 }
                 }
         }      
}
