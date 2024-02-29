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
                mail bcc: ", body: 'Hello, This is an email from jenkins pipeline.', cc: ", from: ", reply To: ",
                    subject: 'EmailJenkinsPipeline', to: 'rash12342504@gmail.com' }


        // Add more stages as needed
    }


}
}
