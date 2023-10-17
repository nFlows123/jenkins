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
        stage('Run PowerShell Script') {
            steps {
                // This step runs the PowerShell script
                sh 'sh1_file.sh'
            }
        }
    }
}
