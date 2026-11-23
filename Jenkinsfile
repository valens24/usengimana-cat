pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                git branch: 'main',
                    url: 'https://github.com/valens24/usengimana-cat.git'
            }
        }

        stage('Docker Image') {
            steps {
                sh 'docker images usengimana/usengimana-cat:v6'
            }
        }

        stage('Verify Project') {
            steps {
                sh 'ls -la'
                sh 'test -f package.json'
            }
        }
    }
}
