pipeline {
    agent any

    stages {
        stage('Clone Repo') {
            steps {
                git 'https://github.com/USERNAME/hello-jenkins.git'
            }
        }

        stage('Run Script') {
            steps {
                sh 'bash script.sh'
            }
        }
    }
}