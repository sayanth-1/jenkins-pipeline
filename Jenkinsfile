pipeline {
    agent any

    stages {

        stage('Build') {
            steps {
                bat 'echo Building application'
                bat 'dir'
            }
        }

        stage('Docker Build') {
            steps {
                bat 'docker build -t jenkins-docker-demo .'
            }
        }

        stage('Test') {
            steps {
                bat 'docker images'
            }
        }

        stage('Deploy') {
            steps {
                bat 'docker rm -f jenkins-docker-demo-container 2>nul || exit /b 0'
                bat 'docker run -d -p 8082:80 --name jenkins-docker-demo-container jenkins-docker-demo:latest'
            }
        }
    }
}
