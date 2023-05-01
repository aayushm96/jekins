pipeline {
	agent any
	stages {
		stage ('stage 1') {
			steps {
				echo "This is stage 1"
				checkout scmGit(branches: [[name: '*/master']], extensions: [], userRemoteConfigs: [[url: 'https://github.com/aayushm96/onlinebookstore.git']])
				mvn clean install 
			}
		}
		stage ('stage 2') {
			steps {
				echo "This is stage 2"
			}
		}
	}
}
