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
		
		stage('Build') {
            steps {
                java -version
            }
        }
        
        stage('Five') {
			steps {
				echo 'Finished'
			}
		}		
	}
}
