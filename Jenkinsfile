pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                sh 'g++ -o obj PES1UG20CS684.cpp'
                build job : 'PES1UG20CS684-1'
                echo 'Build stage successful'
            }
        }
        stage('Test') {
            steps {
                sh './obj1'
                echo 'Test stage successful'
            }
        }
        stage('Deploy') {
            steps {
                sh 'echo "Deploying "'
                echo 'Deployment successful'
            }
        }
    }
    post {
        failure {
          echo 'Pipeline failed'
                }
            
        
    }
}
