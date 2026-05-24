pipeline {
    agent any

    stages {

        stage('Clone Repository') {
            steps {
                git branch: 'main', url: 'https://github.com/srushtideshmukh44/ai-resume-analyzer.git'
            }
        }

        stage('Check Files') {
            steps {
                sh 'ls -la'
                sh 'ls backend'
                sh 'ls frontend'
            }
        }

        stage('Build Success') {
            steps {
                echo 'Jenkins Pipeline Working Successfully'
            }
        }
    }
}