pipeline {
         agent any
         
         stages {
                 stage('One') {
                 steps {
                          script{
                             def a="release/3.4.0"
                             def b=a.split("/")
                                   bat 'echo ${b}'
                          }
              
                 }
                 }
         }      
}
