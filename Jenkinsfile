pipeline {
	agent none
		stages {
			stage('Back-end') {
				agent {
					docker { image 'nginx' }
				}
				steps {
					sh 'ls -al'
				}
			}
				stage('Front-end') {
					agent {
						docker { image 'node:7-alpine' }
					}
				steps {
					sh 'node --version'
				}
			}
		}
}
