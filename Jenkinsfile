pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                echo "Github"
            }
        }

        stage('Build') {
            steps {
                echo "Building the application..."
   
            }
        }

        stage('Test') {
            steps {
                echo "Running unit tests..."
          
            }
        }

        stage('Archive') {
            steps {
                echo "Archiving build artifacts..."
            }
        }
    }

    post {
        success {
            echo 'Build completed successfully.'
        }
        failure {
            echo 'Build failed.'
        }
        always {
            echo 'This block runs no matter what.'
        }
    }
}
