pipeline {
	agent any
	stages {

		stage('Build') {
			steps {
				echo "Build"
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
		success {
			echo 'Jenkins Job Success!'
		}
		failure {
			echo 'Jenkins Job Failed.'
		}
	}
}
