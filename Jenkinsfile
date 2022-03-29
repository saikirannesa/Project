pipeline {
    agent any
		tools {
		  git 'Git'
		  maven 'M2_HOME'
		  jdk 'JAVA_HOME'
		  }
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




