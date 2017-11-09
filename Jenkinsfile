stage('Version') {
    node {
        checkout scm
        sh 'pwd'
        sh 'ls -la'
        sh 'docker run --rm --name builder-container node npm -v'
		sh 'echo ${env.WORKSPACE}'
        sh 'docker run --rm --name builder-container -v "${pwd}":/opt -w /opt node npm install'
    }
}