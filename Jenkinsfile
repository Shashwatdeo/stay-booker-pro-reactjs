pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                checkout scm
            }
        }

        stage('Build Docker Image') {
            steps {
                script {
                    docker.build('hotel-booking-app')
                }
            }
        }

        stage('Run Tests') {
            steps {
                script {
                    // Add any test steps here if needed, for example:
                    // docker.image('hotel-booking-app').inside {
                    //     sh 'npm test'
                    // }
                }
            }
        }

        stage('Deploy') {
            steps {
                script {
                    // Add deployment steps here
                }
            }
        }
    }
}
