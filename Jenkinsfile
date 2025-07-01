pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                git branch: 'main', url: 'https://github.com/ishwarthia/ci-cd-php-app.git'
            }
        }

        stage('Build') {
            steps {
                sh 'php -v'
            }
        }

        stage('Test') {
            steps {
                sh 'phpunit tests'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying application...'
                // Add real deploy command here
            }
        }
    }
}
