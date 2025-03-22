pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                script {
                    echo "Building the project..."
                    sh 'g++ -o hello_exec hello.cpp' // Compile the C++ file
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
