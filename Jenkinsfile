
pipeline {
    agent any

    stages {

        stage('Checkout') {
            steps {
                echo 'Getting Java code from GitHub'
            }
        }

        stage('Compile') {
            steps {
                bat 'javac hello.java'
            }
        }

        stage('Run') {
            steps {
                bat 'java hello'
            }
        }
    }

    post {
        success {
            echo 'Java Program Executed Successfully!'
        }

        failure {
            echo 'Build Failed!'
        }
    }
}
