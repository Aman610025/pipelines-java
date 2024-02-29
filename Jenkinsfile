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
            emailext bcc: '', 
                     body: 'Hello, This is an email from Jenkins pipeline.', 
                     cc: '', 
                     from: 'rash12342504@gmail.co', 
                     replyTo: 'rash12342504@gmail.co', 
                     subject: 'Email JenkinsPipeline', 
                     to: 'rash12342504@gmail.com'
        }
    }
}

}
}
