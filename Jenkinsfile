pipeline {
	agent any
	stages {
		stage('Build') {
			steps {
				echo 'Runnig build automation'
				sh './gradlew build --no-deamon'
				archiveArtifacts artifacts: 'dist/trainSchedule.zip'
			}
		}
	}
}
