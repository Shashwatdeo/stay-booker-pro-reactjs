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
                    docker.build('hotel-booking-app:latest')
                }
            }
        }

        stage('Done') {
            steps {
                echo 'Pipeline executed successfully!'
            }
        }
    }
}
