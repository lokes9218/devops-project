
pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                git 'https://github.com/lokes9218/devops-project.git'
            }
        }
        stage('Build') {
            steps {
                bat 'mvn clean install'
            }
        }
        stage('Test') {
            steps {
                bat 'mvn test'
            }
        }
    }
}
