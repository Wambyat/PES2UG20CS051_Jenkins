pipeline {
    agent any
    stages {
        stage( 'Build') {
            steps {
                g++ hello.cpp
                echo 'Build Stage Successful '
            }
        }
        stage( 'Test') {
             steps {
                hello.exe
                echo 'Test Stage Successful '
             }
        }
        stage( 'Deploy') {
            steps {
                echo 'Deployment Successful '
            }
        }
    }
    post {
        failure {
            echo 'pipeline failed'
        }
    }
}