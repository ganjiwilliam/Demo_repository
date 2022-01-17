pipeline{
    agent any
    stages{  
	    stage('three'){
		    steps{
			    bat '''
			    mkdir hey
			    xcopy /e /i DemoDirectory hey
			   
			    '''
			    }		  
	    }
    }
    }
