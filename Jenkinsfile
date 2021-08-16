pipeline {
         agent any
         
         stages {
                 stage('One') {
                 steps {
                          script{
                             def a=%GIT_BRANCH%
                             
                                   a=a[8..12]
                                   echo "new value is ${a}"
                          }
              
                 }
                 }
         }      
}
