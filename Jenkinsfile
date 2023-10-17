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
        stage('Run Shell Script') {
            steps {
                // This step runs the Bash script
                sh './sh1_file.sh'
            }
        }
    }
}
