pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                echo 'Checkout'
            }
        }
        
        stage('Initialize') {
            steps {
                sh 'python init.py'
            }
        }
        
        stage('Deploy') {
            steps {
                sh 'python deploy.py'
            }
        }
        
        stage('Finish') {
            steps {
                echo 'Finished.'
            }
        }
    }
}
