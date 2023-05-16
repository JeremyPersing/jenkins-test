pipeline {
    agent {
        any {
            image 'node:lts-bullseye-slim' 
            args '-p 5000:5000' 
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
                sh "npm start &" // add & to run in background
            }
        }
    }
}

