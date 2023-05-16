pipeline {
    agent {
        docker {
            image 'node:lts-bullseye-slim' 
            args '-p 80:5000' 
        }
    }
    stages {
        stage('Build') { 
            steps {
                sh 'npm install' 
            }
        }
        stage('Deploy') {
            steps {
                sh 'npm start'
            }
        }
    }
}

