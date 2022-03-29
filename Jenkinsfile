pipeline {
    agent any
    stages {
        stage('mvn clean') {
            steps {
                echo 'clean..'
            }
        }
        stage('mvn Test') {
            steps {
                echo 'Testing..'
            }
        }
		stage('mvn package') {
			steps {
					echo 'Package..'
			}
		}
        stage('mvn Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}




