pipeline {
    agent any

    environment {
        IMAGE_NAME = 'dipakjid/hello-world-demo'
        DOCKER_CREDENTIALS_ID = 'dockerhub-credentials'
    }

    stages {       
        
        stage('Checkout') {
            steps {
                checkout scm
            }
        }
        
    }
}
