pipeline {
    agent any 
    stages {
        stage('Build') {
            steps {
                echo 'Building...'
                sh './gradlew assemble' // Builds the project
            }
        }
        stage('Test') {
            steps {
                echo 'Running tests...'
                sh './gradlew test' // Runs the test cases
            }
        }
    }
    post {
        always {
            echo 'Pipeline finished.'
        }
    }
}
