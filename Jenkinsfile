pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                checkout scm
            }
        }

        stage('Build and Push Docker Image') {
            steps {
                script {
                    // Build the Docker image
                    def customImage = docker.build("stradegi001/nflowsr2:neo4j4.4.7test")

                    // Push the image to Docker Hub
                    customImage.push()
                }
            }
        }
    }
}
