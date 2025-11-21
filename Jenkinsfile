pipeline {
    agent any

    tools {
        jdk 'Java21'
    }

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
