pipeline {
    agent any
    stages {
        stage('One') {
                steps {
                        echo 'Hi, this is Shubham from Git'
			
                }
        }
	    stage('Two'){
		    
		steps {
			echo 'Hi, this is Jenkins from Git'
        }
	    }
        stage('Three') {
                when {
                        not {
                                branch "master"
                        }
                }
                steps {
			echo "Hello"
                        }
        }
        stage('Four') {
                parallel {
                        stage('Unit Test') {
                                steps{
                                        echo "Running the unit test..."
                                }
                        }
                               
			}  }
        }
    }
