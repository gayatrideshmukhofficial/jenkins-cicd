pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                sh '''
                   echo "Building the project..."
                   javac HelloWorld.java
                '''
            }
        }

        stage('Test') {
            steps {
                sh '''
                   echo "Running tests..."
                   java HelloWorld
                '''
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deployment successful! Your app is running.'
            }
        }
    }
}
