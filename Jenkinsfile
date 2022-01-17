
pipeline{
    agent any
    stages{         
        stage('one'){
            steps{     
		    bat 'mkdir hello1'
                    cleanWs()
		    
		    bat 'mkdir hello2'
                                                   
	        }    
            }
	    stage('two'){
            steps{     
		    bat '''mkdir hello3
		    cd hello3
		    '''
		    cleanWs()
                    bat 'mkdir hello3'
                                                   
	        }    
            }
	    stage('three'){
		    steps{
			    ws('DemoDirectory'){
				    bat 'mkdir hello4'
			    }
    }
    }
