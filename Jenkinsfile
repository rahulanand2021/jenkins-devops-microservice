pipeline {
	agent any

	stages {
		stage('Build') {
			steps{
				echo "Build"
				echo "PATH is $PATH"
				echo "BUILD NUMBER is env.BUILD_NUMBER"
				echo "BUILD ID is env.BUILD_ID"
				echo "JOB Name is env.JOB_NAME"
				echo "BUILD TAG IS env.BUILD_TAG"
				echo "BUILD URL IS env.BUILD_URL"

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
