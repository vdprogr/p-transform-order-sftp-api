pipeline {

	agent any
	stages {
		stage('Build') {
			steps {
				bat 'mvn -B -U -e -V clean -DskipTests package'
			}
		}
			stage('Test') {
			steps {
				bat 'echo ********** tests skipped **********'
			}
		}
		
			stage('Deployment') {
			steps {
				bat 'mvn -U -V -e -B -DskipTests deploy -DmuleDeploy   -Danypoint.username=ractice -Danypoint.password=practiCE1! -DmuleDeploy -Dencryption.key=Vital+2024'
			}
		}
	}
}