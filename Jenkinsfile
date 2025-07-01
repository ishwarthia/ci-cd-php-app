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
                echo 'Building the application...'
                // Add your PHP build commands here
            }
        }

        stage('Test') {
            steps {
                echo 'Running tests...'
                // Add your test command like: sh 'vendor/bin/phpunit tests'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying application...'
                // Add deployment commands here
            }
        }
    }
}
