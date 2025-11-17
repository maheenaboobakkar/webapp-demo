pipeline {
    agent any

    stages {
        stage('Check Node.js & npm') {
            steps {
                sh '/usr/bin/node -v'
                sh '/usr/bin/npm -v'
            }
        }

        stage('Install Dependencies') {
            steps {
                sh '/usr/bin/npm install'
            }
        }

        stage('Test') {
            steps {
                sh '/usr/bin/npm test'
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
