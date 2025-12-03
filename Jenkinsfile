pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                git branch: 'dev',
                    credentialsId: 'token',
                    url: 'https://github.com/ravikumara004/acc.git'
            }
        }

        stage('Build') {
            steps {
                sh 'echo from dev Building application'
            }
        }

        stage('Test') {
            steps {
                sh 'echo dev Running tests'
            }
        }

        stage('Deploy') {
            steps {
                sh 'echo from dev Deploying application'
            }
        }
    }
}
