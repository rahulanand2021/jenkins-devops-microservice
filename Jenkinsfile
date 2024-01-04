pipeline {
	agent any
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
