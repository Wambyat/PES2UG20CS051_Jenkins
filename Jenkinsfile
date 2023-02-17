pipeline {
    agent any
    stages {
        stage( 'Build') {
            steps {
                sh 'g++ hello.cpp'
                echo 'Build Stage Successful '
            }
        }
        stage( 'Test') {
             steps {
                sh './hello'
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
