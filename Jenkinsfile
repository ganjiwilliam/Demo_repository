pipeline {
         agent any
         environment{
                  a="williamcarey"
         }
         stages {
                 stage('One') {
                 steps {
                          script{
                             def a="release/3.4.0"
                             def b=a.split("/")
                                   echo "splitted value is   ${b}"
                                   a=a[7..11]
                                   echo "new value is ${a}"
                          }
              
                 }
                 }
         }      
}
