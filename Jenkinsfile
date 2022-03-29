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
						sh 'mvn Compile'
						echo 'Compiling..'
            }
        }
        stage('mvn Test') {
            steps {
						sh 'mvn Test'
						echo 'Testing..'
            }
        }
		stage('mvn Package') {
			steps {
						sh 'mvn Package'
						echo 'Package..'
			}
		}
		stage('mvn Verify') {
            steps {
						sh 'mvn Verify'
						echo 'Verifying..'
            }
        }
		stage('mvn SONAR SCAN') {
            steps {
						sh 'mvn SONAR SCAN'
						echo 'SONAR SCAN..'
            }
        }
        stage('mvn Deploy') {
            steps {
						sh 'mvn Deploy'
						echo 'Deploying..'
            }
        }
    }
}




