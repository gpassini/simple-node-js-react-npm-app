stage('Version') {
    node {
        checkout scm
        sh 'pwd'
        sh 'ls -la'
        sh 'docker run --rm --name builder-container node npm -v'
        sh 'docker volume create node-modules'
		sh 'echo ${env.WORKSPACE}'
        sh 'docker run --rm --name builder-container -v ${env.WORKSPACE}:/opt -w /opt node npm install'
    }
}