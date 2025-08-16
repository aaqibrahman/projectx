pipeline {
    agent any

    environment {
        // Replace with your public GitHub repo URL
        GIT_REPO = 'https://github.com/aaqibrahman/projectx.git'
    }

    stages {
        stage('Checkout') {
            steps {
                // Grab the latest code from GitHub (no credentials needed for public repo)
                git url: "${GIT_REPO}", branch: 'main'
            }
        }

        stage('Build') {
            steps {
                // Simulate building your project
                echo "Building the project..."
            }
        }

        stage('Test') {
            steps {
                // Simulate running tests
                echo "Running tests..."
            }
        }
    }

    post {
        success {
            echo '✅ Build and tests successful!'
        }
        failure {
            echo '❌ Build or tests failed!'
        }
    }
}
