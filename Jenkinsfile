# Jenkinsfile  - Declarative Jenkins pipeline script for your CI/CD process.

pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                sh 'python -m pip install -r requirements.txt'
            }
        }
        stage('Test') {
            steps {
                sh 'python -m pytest tests/'
            }
        }
        stage('Deploy') {
            steps {
                // Add deployment steps here, e.g., deploying to a server or cloud platform.
            }
        }
    }

    post {
        always {
            cleanWs()
        }
    }
}
