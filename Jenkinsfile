pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                // Compile the .cpp file
                sh 'g++ PES1UG22CS626-1.cpp -o PES1UG22CS626-1'
                echo 'Build Stage Successful'
            }
        }
        stage('Test') {
            steps {
                // Print output of the .cpp file
                sh './PES1UG22CS626-1'
                echo 'Test Stage Successful'
            }
        }
        stage('Deploy') {
            steps {
                // Deployment steps (if any)
                echo 'Deployment Successful'
            }
        }
    }
    post {
        failure {
            echo 'Pipeline failed'
        }
    }
}
