pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                git 'https://github.com/KshitijMahale/clouddefaulter.git'
            }
        }

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
