pipeline {
	agent any
	stages {
		stage('One') {
			steps {
				echo 'Hi, this is Soumitra from roytuts'
			}
		}
		
		stage('Two') {
			steps {
				input('Do you want to proceed?')
			}
		}
		
	stage('Java') {
            steps {
                  bat 'java -version'
            }
        }
        stage('Go') {
            steps {
                  bat 'go version'
            }
        }
        stage('Five') {
			steps {
				echo 'Finished'
			}
		}		
	}
}
