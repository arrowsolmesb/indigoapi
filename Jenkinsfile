pipeline {

  agent any
  stages {
		stage('Build Application') {
		  steps {
				bat 'mvn clean install'
		  }
		}
		stage('Deploy Application into standalone') {
		  steps {
			  bat "mvn deploy -P standalone"
		  }
		}
	}
}	