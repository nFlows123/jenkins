pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                // This step checks out the code from the repository
                script {
                    checkout scm
                }
            }
        }
        stage('Prepare and Run Shell Script') {
            steps {
                script {
                    // Grant execute permission to the script
                    sh 'chmod +x sh1_file.sh'
                    
                    // Run the Bash script
                    sh './sh1_file.sh'

                    sh 'docker build --no-cache -t stradegi001/nflowsr2:neo4j4.4.7test -f Neo4jDockerFile .'
                }
            }
        }
    }
}
