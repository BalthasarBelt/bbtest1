pipeline {
	agent none
    stage('Clone repository') {
        /* Let's make sure we have the repository cloned to our workspace */

        checkout scm
    }

    stage('Build image') {
        /* This builds the actual image; synonymous to
         * docker build on the command line */
		agent { image 'maven:3.8.1-adoptopenjdk-11' }
		steps { sh 'mvn --version' }
        /* app = docker.build("balthasarbelt/bbtest1") */
    }

}
