pipeline {
    agent any
    stages {
        stage('mvn Clean') {
            steps {
                echo 'Clean..'
            }
        }
		stage('mvn Validate') {
            steps {
                echo 'Validating..'
            }
        }
		stage('mvn Compile') {
            steps {
                echo 'Compiling..'
            }
        }
        stage('mvn Test') {
            steps {
                echo 'Testing..'
            }
        }
		stage('mvn Package') {
			steps {
					echo 'Package..'
			}
		}
		stage('mvn Verify') {
            steps {
                echo 'Verifying..'
            }
        }
		stage('mvn SONAR SCAN') {
            steps {
                echo 'SONAR SCAN..'
            }
        }
        stage('mvn Deploy') {
            steps {
                echo 'Deploying..'
            }
        }
    }
}




