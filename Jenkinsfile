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
                }
            }
        }
    }
}
