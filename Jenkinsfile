pipeline {
	agent any 
	stages {
		stage('stages running parallel') {
			failFast true 
			parallel {
				stage('stage1') {
					when {
						branch 'dev'
					}
					steps {
						echo 'Stage1 is running'
						sleep 10
					}
				} 
				stage('stage2'){
					steps {
						echo 'Stage2 is running'
						sleep 10
					}
				}
				stage('stage3'){
					steps {
						echo 'Stage3 is running'
						sleep 10
					}
				}
			}
		}
	}
}