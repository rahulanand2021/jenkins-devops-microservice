pipeline {
//	agent any
	agent { docker { image 'maven:3.6.3' } }
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
