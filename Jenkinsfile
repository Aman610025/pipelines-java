pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                // Build your project (e.g., with Maven)
                sh 'mvn clean compile'
            }
        }
        stage('Test') {
            steps {
                // Run tests (e.g., with Maven)
                sh 'mvn test'
            }
        }
        // Add more stages as needed
    }
    post {
        always {
            // Send email notification with pipeline status
            emailext subject: 'Pipeline Status',
                     body: 'The pipeline status is: ${currentBuild.currentResult}',
                     recipientProviders: [culprits(), developers()]
        }
    }
}
