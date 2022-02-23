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
				branch 'test'
			}
			steps {
				echo 'Building dev'
			}
		}
		stage('Build default') {
			steps {
				echo 'Building default'
			}
		}
	}
}
