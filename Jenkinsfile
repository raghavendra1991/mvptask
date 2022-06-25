// Declarative pipeline
pipeline {
    agent any

    environment {
        http_proxy = 'http://127.0.0.1:3128/'
        https_proxy = 'http://127.0.0.1:3128/'
        ftp_proxy = 'http://127.0.0.1:3128/'
        socks_proxy = 'socks://127.0.0.1:3128/'
    }

    stages {
        
        stage ('Build Docker Image') {
            steps {
                echo 'Build Multiple Docker Image Using Docker-Compose'
                sh 'docker-compose build'       
            }
        }
    }
}
