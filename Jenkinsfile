pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building the Gradle project...'
                sh './gradlew clean build'
            }
        }

        stage('Test') {
            steps {
                echo 'Running tests...'
                sh './gradlew test'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deployment stage (optional)'
            }
        }
    }
}
