pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                git 'https://github.com/hermannbrice12/projet-maven.git'
            }
        }
        stage('Build') {
            steps {
                sh 'mvn clean package'
            }
        }
        stage('Test') {
            steps {
                sh 'mvn test'
            }
        }
    }
}
