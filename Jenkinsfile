pipeline {
	agent { docker { image 'node:13.8' } }
	stages {

		stage('Build') {
			steps {
				echo "Build"
			    sh 'node --version'
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
		changed {
			echo 'Changed no idea from what to what'
		}
	}
}
