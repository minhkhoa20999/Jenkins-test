pipeline {
	agent any 
	stages {
		stage('Build master') {
			when {
				branch 'master'
			}
			steps {
				echo 'Building master'
			}
		}
		stage('Build dev') {
			when {
				branch 'dev'
			}
			steps {
				echo 'Building dev'
			}
		}
	}
}