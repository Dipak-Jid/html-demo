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
        
        stage('Build Docker Image') {            
            agent {
                docker {
                    image 'ubuntu:22.04'        // or any image with Docker/Java installed
                    args '-u root'              // Run as root user
                }
            }
            steps {
                sh 'docker build -t hello-world-demo .'
            }
        }        
        
    }
}
