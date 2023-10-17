pipeline {
    agent any

    stages {
        stage('Build and Push Docker Image') {
            steps {
                script {
                    echo "hello"
                    sh 'docker build --no-cache -t stradegi001/nflowsr2:neo4j4.4.7test -f Neo4jDockerFile .'
                    sh 'docker push stradegi001/nflowsr2:neo4j4.4.7test'
                }
            }
        }
    }
}
