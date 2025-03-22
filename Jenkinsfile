pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building the application...'
            }
        }

        stage('Test') {
            steps {
                echo 'Running tests...'
            }
        }

        stage('Deploy') {
            steps {
                script {
                    echo 'Deploying application...'
                    error('Deployment Failed!') // Simulates a deployment failure
                }
            }
        }
    }
}
