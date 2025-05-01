pipeline {
    agent any
    
    stages {
        stage('Build') {
            steps {
                script {
                    sh 'g++ -o hello_exec main/PES1UG22AM161.cpp'
                }
            }
        }
        
        stage('Test') {
            steps {
                script {
                    sh './hello_exec'
                }
            }
        }
        
        stage('Deploy') {
            steps {
                script {
                    echo 'Deploying the application!'
                  
                }
            }
        }
    }
    
    post {
        failure {
            echo 'Pipeline failed :('
        }
    }
}