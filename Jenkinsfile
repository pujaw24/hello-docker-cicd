pipeline {
    agent any

    stages {

        stage('Build Docker Image') {
            steps {
                sh 'docker build -t hello-docker-app .'
            }
        }

        stage('Run Container') {
            steps {
                sh 'docker run hello-docker-app'
            }
        }
    }
}