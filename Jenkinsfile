stage('test') {
	node {
	    checkout scm
	    sh "docker run --rm --name testing-container npm install"
	}
}