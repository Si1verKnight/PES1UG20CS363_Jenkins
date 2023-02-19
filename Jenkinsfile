// Code/script written to create basic pipeline using GitHub repository
pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                sh 'g++ Cloud.cpp'
                build 'PES1UG20CS363-1'
                echo 'Build stage successful'
            }
        }
        stage('Test') {
            steps {
                sh './a.out'
                // sh '.aout'
                echo 'Test stage successful'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deployment stage successful'
            }
        }
    }
    post {
        failure {
            echo 'Pipeline Failed.'
        }
    }
}



