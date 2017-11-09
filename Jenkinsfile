stage('Version') {
    node {
        checkout scm
        sh 'pwd'
        sh 'ls -la'
        sh 'docker run --rm --name builder-container node npm -v'
		sh 'echo "Will try to install"'
        sh 'docker run --rm --name builder-container -v /var/lib/jenkins/workspace/simple-node-js-react-npm-app:/opt -w /opt node npm install'
    }
}