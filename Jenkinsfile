pipeline {
    agent any

    stages {
        stage('Clone') {
            steps {
                git 'https://github.com/maheenaboobakkar/webapp-demo.git'
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
