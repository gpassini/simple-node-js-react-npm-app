stage('Version') {
    node {
        checkout scm
        sh 'pwd'
        sh 'ls -la'
        sh 'docker run --rm --name builder-container node npm -v'
        sh 'docker run --rm --name builder-container node npm install'
    }
}