// pipeline {
//     agent {
//         docker {
//             image 'node:18-bullseye-slim' 
//             // args '-p 80:5000' 
//         }
//     }
//     stages {
//         stage('Build') { 
//             steps {
//                sh 'npm install'
//             }
//         }
//         stage('Deploy') {
//             steps {
//                 sh 'npm start'
//             }
//         }
//     }
// }



pipeline {
    agent {
        docker {
            image 'node:lts-bullseye-slim' 
            args '-p 3000:3000' 
        }
    }
    stages {
        stage('Build') { 
            steps {
                sh 'npm install' 
            }
        }
    }
}

