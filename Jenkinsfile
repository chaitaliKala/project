// Jenkinsfile
pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                // Clone the repository containing the code
                git 'https://github.com/chaitaliKala/project.git'
            }
        }
        stage('Build') {
            steps {
                // Compile the Java application
                sh 'javac Main.java'
            }
        }
        stage('Run') {
            steps {
                // Run the compiled Java application
                sh 'java Main'
            }
        }
    }
    post {
        always {
            echo 'Pipeline execution completed.'
        }
    }
}
