
pipeline{
    agent any
    stages{         
        stage('one'){
            steps{     
		    bat 'mkdir hello1'
                    cleanWs()
		    echo "${ENV_NAME}"
		    bat 'mkdir hello2'
                                                   
	        }    
            }
	    stage('two'){
            steps{     
		    bat 'mkdir hello3'
                    
                                                   
	        }    
            }
    }
