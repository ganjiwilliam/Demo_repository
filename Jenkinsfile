pipeline{
    agent any
    stages{  
	    stage('three'){
		    steps{
			    bat '''
			    mkdir hey
			    xcopy /e /i DemoDirectory hey
			    echo hello william > hello11.txt
			    '''
			    }		  
	    }
    }
    }
