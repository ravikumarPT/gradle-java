pipeline {
    // install golang 1.14 on Jenkins node
    agent any
    tools {
        go 'go1.14'
    }
    environment {
        GO114MODULE = 'on'
        CGO_ENABLED = 0 
        GOPATH = "${JENKINS_HOME}/jobs/${JOB_NAME}/builds/${BUILD_ID}"
    }
    stages {
        stage("Go Version") {
            steps {
                echo 'go version is here'
                bat 'go version'
            }
        }
        stage('Go Make') {
		    steps {
			  echo 'TEST EXECUTION STARTED'
			  bat 'make run'
		    }
		}
    }
}
