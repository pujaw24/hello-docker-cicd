stage('Run Container') {
    steps {
        sh 'docker rm -f hello-container || true'
        sh 'docker run -d --name hello-container -p 8000:8000 hello-docker-app'
    }
}