
pipeline {
    agent any

    environment {
        DEPLOY_TARGET = 'staging'
    }

    stages {
        stage('Build') {
            steps {
                echo 'Building the application...'
                sh 'echo "Compiling source code..."'
                echo 'Running $BRANCH_NAME pipeline'
            }
        }

        stage('Test') {
            steps {
                echo 'Testing the application...'
                sh 'echo "Running unit tests..."'
            }
        }

        stage('Deploy') {
            steps {
                echo "Deploying to ${env.DEPLOY_TARGET}..."
                sh 'echo "Application deployed successfully!"'
            }
        }
    }
}
