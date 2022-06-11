pipeline {
	agent {
        docker { image 'node:16.13.1-alpine' }
    }
	stages {
    stage('Clone repository') {
        steps {
			checkout scm
		}
    }
	}
}
