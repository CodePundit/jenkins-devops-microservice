pipeline {
	agent any
	// agent { docker { image 'node:13.8' } }
	stages {

		stage('Build') {
			steps {
				echo "Build"
			    // sh 'node --version'
				echo "PATH = $PATH"
				echo "env.JOB_NAME = $env.JOB_NAME"
				echo "env.JOB_URL = $env.JOB_URL"
				echo "env.BUILD_TAG = $env.BUILD_TAG"
				echo "env.BUILD_ID = $env.BUILD_ID"
				echo "env.BUILD_NUMBER = $env.BUILD_NUMBER"
			}
		}
		stage('Test') {
			steps {
				echo "Test"
			}
		}
	}
	post {
		always {
			echo 'Always'
		}		
		changed {
			echo 'Changed no idea from what to what'
		}
		failure {
			echo 'Jenkins Job Failed.'
		}
		success {
			echo 'Jenkins Job Success!'
		}
	}
}
