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
                bat 'python init.py'
            }
        }
        
        stage('Deploy') {
            steps {
                bat 'python deploy.py'
            }
        }
        
        stage('Finish') {
            steps {
                echo 'Finished.'
            }
        }
    }
}
