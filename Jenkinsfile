pipeline {
    agent any

    stage('Build') {
    steps {
        script {
            echo "Building the project..."
            sh 'g++ -o hello_exec hello_error.cpp' // Intentional error (file doesn't exist)
        }
    }
}

        stage('Test') {
            steps {
                script {
                    echo "Running tests..."
                    sh './hello_exec' // Run the compiled C++ program
                }
            }
        }

        stage('Deploy') {
            steps {
                script {
                    echo "Deploying the application..."
                    // Placeholder for deployment commands
                }
            }
        }
    }

    post {
        failure {
            echo "Pipeline failed "
        }
        success {
            echo "Pipeline executed successfully "
        }
    }
}
