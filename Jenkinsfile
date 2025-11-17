pipeline {
    agent any

    environment {
        // Add Node.js and npm to PATH explicitly
        PATH = "/usr/bin:$PATH"
    }

    stages {
        stage('Check Node.js & npm') {
            steps {
                sh 'echo "Node path: $(which node)"'
                sh 'echo "npm path: $(which npm)"'
                sh 'node -v'
                sh 'npm -v'
            }
        }

        stage('Install Dependencies') {
            steps {
                sh 'npm install'
            }
        }

        stage('Test') {
            steps {
                sh 'npm test'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Simulating Deployment...'
            }
        }

        stage('Monitoring') {
            steps {
                echo 'Simulating Monitoring...'
            }
        }
    }

    post {
        always {
            echo 'Pipeline completed.'
        }
    }
}
