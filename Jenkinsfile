pipeline {
    agent any
				tools {
				git 'Git' git credentialsId: 'GitHub', url: 'https://github.com/saikirannesa/Project.git'
				jdk 'JAVA_HOME'
				maven 'M2_HOME'
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




