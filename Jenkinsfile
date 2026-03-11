pipeline {
    agent any

    stages {
        stage('Clone Repo') {
            steps {
                git 'https://github.com/HiragiIsMe/hello-jenkins.git'
            }
        }

        stage('Run Script') {
            steps {
                sh 'bash script.sh'
            }
        }
    }
}
