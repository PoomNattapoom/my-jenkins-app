pipeline {
    agent any

    tools {
        nodejs "NodeJS 16" // Set this in Jenkins tools config
    }

    stages {
        stage('Clone') {
            steps {
                git 'https://github.com/PoomNattapoom/my-jenkins-app.git'
            }
        }

        stage('Install Dependencies') {
            steps {
                sh 'npm install'
            }
        }

        stage('Build') {
            steps {
                echo 'No build step for now'
            }
        }

        stage('Test') {
            steps {
                echo 'No tests yet'
            }
        }

        stage('Run App') {
            steps {
                sh 'nohup npm start &'
                echo 'App is running in background'
            }
        }
    }
}
