pipeline {
         agent any
         
         stages {
                 stage('One') {
                 steps {
                          script{
                             def a="release/3.4.0"
                             
                                   a=a[8..12]
                                   echo "new value is ${a}"
                          }
              
                 }
                 }
         }      
}
