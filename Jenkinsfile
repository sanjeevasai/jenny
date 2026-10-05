pipeline {
    agent any

    stages {

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
            echo 'Java program executed successfully!'
        }

        failure {
            echo 'Java program failed!'
        }
    }
}
