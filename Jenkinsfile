pipeline {
    agent any
    stages {
        stage( 'Build') {
            steps {
                echo 'Build Stage Successful '
            }
        }
        stage( 'Test') {
             steps {
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