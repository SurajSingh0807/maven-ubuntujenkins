pipeline{
    agent any
    stages{
        stage('Checkout'){
            steps{
                echo 'Checking out code...'
            }
        }
        stage('Build'){
            steps{
                echo 'Building...'
            }
        }
        stage('Test'){
            steps{
                echo 'Testing...'
            }
        }
        stage('Package'){
            steps{
                echo 'Packaging...'
            }
        }
    }
    post {
        success {
            echo 'Build completed successfully!'
        }

        failure {
            echo 'Build failed!'
        }
    }
}