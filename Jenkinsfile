pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                git 'https://github.com/Anu-Mernstack/fullstack-jenkins.git'
            }
        }

        stage('Build Backend') {
            steps {
                echo 'Building backend...'
                sh 'echo Simulated backend build'
            }
        }

        stage('Build Frontend') {
            steps {
                echo 'Building frontend...'
                sh 'echo Simulated frontend build'
            }
        }

        stage('Test') {
            steps {
                echo 'Running tests...'
                sh 'echo All tests passed'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying application...'
                sh 'echo Deployment successful'
            }
        }
    }

    post {
        always {
            echo 'Pipeline finished.'
        }
        success {
            echo 'Build was successful!'
        }
        failure {
            echo 'Build failed.'
        }
    }
}
