pipeline {
    agent any

    stages {

        stage('Checkout') {
            steps {
                git 'https://github.com/rishvanthrr/ex-4.git'
            }
        }

        stage('Build') {
            steps {
                echo 'Building the application'
                sh 'mkdir -p target'
                sh 'echo "Hello CI Pipeline" > target/app.jar'
            }
        }

        stage('Test') {
            steps {
                echo 'Running tests'
            }
        }
    }
}
