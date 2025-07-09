pipeline {
    agent any

    environment {
        APP_NAME = 'MyApp'
    }

    stages {
        stage('📥 Checkout Code') {
            steps {
                echo 'Cloning repo...'
                checkout scm
            }
        }

        stage('📦 Install Dependencies') {
            steps {
                echo 'Installing dependencies...'
                bat 'echo Installing packages...'
            }
        }

        stage('🧪 Run Tests') {
            steps {
                echo 'Running tests...'
                bat 'echo All tests passed!'
            }
        }

        stage('🔧 Build') {
            steps {
                echo "Building ${env.APP_NAME}..."
                bat 'echo Build complete!'
            }
        }

        stage('🚀 Deploy') {
            steps {
                echo "Deploying ${env.APP_NAME}..."
                bat 'echo Deployment done!'
            }
        }
    }

    post {
        always {
            echo 'Pipeline finished.'
        }
        success {
            echo '✅ Automation complete: Pipeline succeeded!'
        }
        failure {
            echo '❌ Automation failed: Check logs.'
        }
    }
}
