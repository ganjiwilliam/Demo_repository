pipeline {
         agent any
         stages {
                 stage('One') {
                 steps {
                     echo 'Hi, this is william'
                 }
                 }
                 stage('Two') {
                 steps {
                    echo 'Hi, this is william'
                 }
                 }
                 
                 stage('Four') {
                 parallel { 
                            stage('Unit Test') {
                           steps {
                                echo "Running the unit test..."
                           }
                           }
                            stage('Integration test') {
                              steps {
                                echo "Running the integration test..."
                              }
                           }
                           }
                           }
              }
}
