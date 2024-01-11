pipeline {
//	agent any
	agent {
        docker {
            // Specify the Docker image for the agent
            image 'maven:3.6.3'
            // You can also add other options like label, args, etc.
        }
	}
	stages {
		stage('Build') {
			steps{
				echo "Build"
			}
		}
		stage('Test') {
			steps{
				echo "Test"
			}	
		}

		stage('Integration Test') {
			steps{
				echo "Integration Test"
			}
		}						
	}
	post {
		always {
			echo 'I am awesome. I always RUN'
		}
		success {
			echo 'I RUN when you are SUCCESSFUL'
		}
		failure {
			echo 'I RUN when you FAIL'
		}

	}

}
