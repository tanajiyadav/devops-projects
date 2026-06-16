pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                checkout scm
            }
        }

        stage('Hello World') {
            steps {
                echo 'Hello World from Jenkins! main branch'
            }
        }
    }

    post {
        success {
            echo 'Build completed successfully.'
        }

        failure {
            echo 'Build failed.'
        }

        always {
            echo 'Pipeline execution finished.'
        }
    }
}
