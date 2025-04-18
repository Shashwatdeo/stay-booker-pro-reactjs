pipeline {
    agent any

    stages {
        stage('Clone') {
            steps {
                echo 'Cloning repository...'
            }
        }

        stage('Build Docker Image') {
            steps {
                script {
                    sh 'docker build -t hotel-booking-app:latest .'
                }
            }
        }

        stage('Run Container') {
            steps {
                script {
                    sh 'docker run -d -p 3000:3000 hotel-booking-app:latest'
                }
            }
        }

        stage('Done') {
            steps {
                echo 'Build and Run complete!'
            }
        }
    }
}
