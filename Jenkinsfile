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
    }
}
        }
    }
}
