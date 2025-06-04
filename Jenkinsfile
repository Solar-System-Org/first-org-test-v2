pipeline {
    agent any

    environment {
        // Example environment variables
        // JAVA_HOME = "/usr/lib/jvm/java-11-openjdk"
        // PATH = "${env.JAVA_HOME}/bin:${env.PATH}"
      echo "Java_home and PATH"
    }

    options {
        // Keep only the 10 most recent builds
        // buildDiscarder(logRotator(numToKeepStr: '10'))
        echo "timestamps"
    }

    triggers {
        // Poll the Git repository every 15 minutes
        echo "pollSCM('H/15 * * * *')"
    }

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
