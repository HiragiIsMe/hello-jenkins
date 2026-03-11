pipeline {
    agent any

    stages {

        stage('Install Dependencies') {
            steps {
                git branch: 'main', url: 'https://github.com/HiragiIsMe/hello-jenkins.git'
            }
        }

        stage('Laravel Setup') {
            steps {
                sh 'echo Hello from Jenkins'
            }
        }

        stage('Run Laravel Server') {
            steps {
                sh 'php artisan serve --host=0.0.0.0 --port=8000 &'
            }
        }

    }
}
