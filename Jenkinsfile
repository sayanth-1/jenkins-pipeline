pipeline {
    agent any

    stages {

        stage('Build') {
            steps {
                bat 'echo Building application'
                bat 'dir'
            }
        }

        stage('Test') {
            steps {
                bat 'echo Running tests'
            }
        }

        stage('Deploy') {
            steps {
                bat 'echo Deploying application'
            }
        }
    }
}
