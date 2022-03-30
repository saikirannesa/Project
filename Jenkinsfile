pipeline {
    agent any
	tools {
			git 'Git'
			jdk 'JAVA_HOME'
			maven 'M2_HOME'
		  }
    stages {
        stage('mvn Clean') {
            steps {
						sh 'mvn clean'
						echo 'Clean..'
            }
        }
		stage('mvn Validate') {
            steps {
						sh 'mvn validate'
						echo 'Validating..'
            }
        }
		stage('mvn Compile') {
            steps {
						sh 'mvn compile'
						echo 'Compiling..'
            }
        }
        stage('mvn Test') {
            steps {
						sh 'mvn test'
						echo 'Testing..'
            }
        }
		stage('mvn Package') {
			steps {
						sh 'mvn package'
						echo 'Package..'
			}
		}
		stage('mvn SONAR SCAN') {
            steps {
						sh 'mvn integration-test'
						echo 'SONAR SCAN..'
            }
        }
		stage('mvn Verify') {
            steps {
						sh 'mvn verify'
						echo 'Verifying..'
            }
        }
		stage('mvn Install') {
            steps {
						sh 'mvn install'
						echo 'Installing..'
            }
        }
    }
}





