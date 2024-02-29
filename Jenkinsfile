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
        stage('Email JenkinsPipeline') {
    steps {
        script {
            emailext (
                to: 'rash12342504@gmail.com',
                subject: 'Email JenkinsPipeline',
                body: 'Hello, This is an email from Jenkins pipeline.',
                mimeType: 'text/plain',
                replyTo: 'rash12342504@gmail.com',
                from: 'rash12342504@gmail.com'
            )
        }
    }
}

}
}
