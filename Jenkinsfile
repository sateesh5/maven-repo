pipeline {
	agent any

	tools {
	  maven "mvn"
	}

	stages{
	  stage("Build") {
	    steps {
	      sh "mvn -version"
	      sh "mvn clean install"

	    }
	  }
	}

	post {
	  always {
	    cleanWS ()
	  }
	}
}
