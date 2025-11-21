pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                sh 'mvn clean install'
            }
        }
    }

    post {
        success {
            echo '✅ Spring Boot project built successfully!'
        }
        failure {
            echo '❌ Build failed'
        }
    }
}
