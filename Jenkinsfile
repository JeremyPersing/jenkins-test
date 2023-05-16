pipeline {
    agent {
        docker {
            image 'node:18-bullseye-slim' 
            args '-p 80:5000' 
        }
    }
    // environment {
    //     HOME = "."
    // }
    stages {
        stage('Build') { 
            steps {
                sh "npm -v"
                sh 'npm install' 
            }
        }
    }
}