pipeline {

    agent any

    stages {

        stage('Checkout') {
            steps {
                echo "Branch = ${env.BRANCH_NAME}"
            }
        }

        stage('Build') {
            steps {
                echo "Building..."
            }
        }

        stage('Test') {
            steps {
                echo "Testing..."
            }
        }

        stage('Deploy') {
            when {
                branch 'main'
            }
            steps {
                echo "Deploying Production..."
            }
        }

    }

    post {

        success {
            echo "SUCCESS"
        }

        failure {
            echo "FAILED"
        }

    }

}