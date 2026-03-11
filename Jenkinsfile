pipeline {
    agent any

    stages {

        stage('Install Dependencies') {
            steps {
                sh 'composer install'
            }
        }

        stage('Laravel Setup') {
            steps {
                sh 'cp .env.example .env'
                sh 'php artisan key:generate'
            }
        }

        stage('Run Laravel Server') {
            steps {
                sh 'php artisan serve --host=0.0.0.0 --port=8000 &'
            }
        }

    }
}