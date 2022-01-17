pipeline{
    agent any
    stages{  
	    stage('three'){
		    steps{
			    bat '''
			    rmdir /s /q hey
			    mkdir hey
			    xcopy /e /i DemoDirectory hey
			   
			    '''
			    }		  
	    }
    }
    }
