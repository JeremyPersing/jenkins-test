pipeline {
    agent {

        docker {
            image 'node:18-bullseye-slim' 
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
                sh 'node index.js'
                echo 'Started server'
            }
        }
    }
}