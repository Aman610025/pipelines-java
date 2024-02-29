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
        mail bcc: '', body: 'This is triggered by git push', cc: '', from: '', replyTo: '', subject: 'Jenkins Pipeline', to: 'rash12342504@gmail.com'
    }
}

}
}
