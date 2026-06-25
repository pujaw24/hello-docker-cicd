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
                sh 'docker rm -f hello-container || true'
                sh 'docker run -d --name hello-container -p 8000:8000 hello-docker-app'
            }
        }
    }
}