pipeline {
    agent any

    tools {
        nodejs 'nodejs16'  // This must match the name you set earlier
    }

    stages {
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
