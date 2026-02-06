pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                // Ovde se koristi credentialsId iz Jenkins Credentials
                git branch: 'main',
                    url: 'git@github.com:zecevicd/jenkins.git',
                    credentialsId: 'f3b2d234-45da-4b9a-a3e7-ba43a4cadb11'
            }
        }

        stage('Build') {
            steps {
                echo 'Hello, world! Build stage radi necega...'
            }
        }

        stage('Test') {
            steps {
                echo 'Pokrećem testove...'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploy pipeline završava!'
            }
        }
    }
}
