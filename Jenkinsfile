pipeline {
	agent none
	stages {
		stage('Build  webhook images') {
			agent {
				dockerfile {
				filename 'Dockerfile'
				dir 'build'
				label 'ansible-server'
				additionalBuildArgs  '--build-arg version=1.0.2'
				}
			}		
		}
	}	
}
