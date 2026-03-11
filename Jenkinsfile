pipeline {
    agent any

    stages {
        stage('Clone Repo') {
            steps {
                git branch: 'main', url: 'https://github.com/HiragiIsMe/hello-jenkins.git'
            }
        }

        stage('Run Script') {
            steps {
                sh 'echo Hello from Jenkins'
            }
        }
    }
}
