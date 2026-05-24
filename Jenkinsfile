pipeline {
    agent any

    stages {

        stage('Clone Repository') {
            steps {
                git 'https://github.com/srushtideshmukh44/ai-resume-analyzer.git'
            }
        }

        stage('Build Backend Docker Image') {
            steps {
                bat 'docker build -t ai-backend ./backend'
            }
        }

        stage('Build Frontend Docker Image') {
            steps {
                bat 'docker build -t ai-frontend ./frontend'
            }
        }

        stage('Docker Compose Up') {
            steps {
                bat 'docker-compose up -d'
            }
        }
    }
}