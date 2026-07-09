pipeline{
    agent any
    stages{
        stage('Checkout'){
            steps{
                echo 'Checking out code...'
                git 'https://github.com/SurajSingh0807/maven-ubuntujenkins.git'
            }
        }
        stage('Build'){
            steps{
                echo 'Building...'
                sh 'mvn compile'
            }
        }
        stage('Test'){
            steps{
                echo 'Testing...'
                sh 'mvn test'
            }
        }
        stage('Package'){
            steps{
                echo 'Packaging...'
                sh 'mvn package'
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