pipeline {
    agent any
    stages {
        stage( 'Build') {
            steps {
                sh 'g++ -o PES2UG20CS051 hello.cpp'
                echo 'Build Stage Successful '
            }
        }
        stage( 'Test') {
             steps {
                sh './PES2UG20CS051'
                echo 'Test Stage Successful '
             }
        }
        stage( 'Deploy') {
            steps {
                //this is intentional error
                ech 'Deployment Successful '
            }
        }
    }
    post {
        failure {
            echo 'pipeline failed'
        }
    }
}
