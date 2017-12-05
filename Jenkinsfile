pipeline {
	agent any
	stages {
		stage('Build') {
			steps {
				bat 'mvn -B -DskipTests clean package'
				bat 'dir'
			}
		}
		stage('Test') {
            steps {
                bat 'mvn test'
            }
        }
	}
}