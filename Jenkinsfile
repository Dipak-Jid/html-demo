pipeline {
    agent any

    environment {
        IMAGE_NAME = 'dipakjid/hello-world-demo'
        DOCKER_CREDENTIALS_ID = 'dockerhub-credentials'
    }

    stages {
        stage('Check Docker Version') {
            steps {
                sh 'docker --version'
            }
        }
        
        stage('Checkout') {
            steps {
                git url: 'https://github.com/Dipak-Jid/html-demo.git', branch: 'master'
            }
        }
    }
}
