pipeline {
    agent any

    stages {
        stage('Clone Repository') {
            steps {
                git branch: 'main', url: 'https://github.com/your-username/your-repo.git'
            }
        }

        stage('Build') {
            steps {
                bat 'javac HelloWorld.java'
            }
        }

        stage('Test') {
            steps {
                bat 'java HelloWorld'
            }
        }

        stage('Deploy') {
            steps {
                bat 'echo Deploying Java application...'
                // Add actual deployment commands here
            }
        }
    }
}
