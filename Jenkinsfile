pipeline {
    agent any

    stages {

        stage('Build Docker Image') {
            steps {
                sh 'docker build -t laravel-app .'
            }
        }

        stage('Run Container') {
            steps {
                sh 'docker stop laravel-app || true'
                sh 'docker rm laravel-app || true'
                sh 'docker run -d -p 9090:8000 --name laravel-app laravel-app'
            }
        }

    }
}