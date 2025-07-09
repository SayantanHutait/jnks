pipeline {
    agent any

    environment {
        // Define any environment variables here
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
                // Simulate install, replace with real command like `npm install` or `pip install -r requirements.txt`
                sh 'echo Installing packages...'
            }
        }

        stage('🧪 Run Tests') {
            steps {
                echo 'Running tests...'
                // Replace with real test command
                sh 'echo All tests passed!'
            }
        }

        stage('🔧 Build') {
            steps {
                echo "Building ${env.APP_NAME}..."
                // Replace with actual build command like `npm run build`
                sh 'echo Build complete!'
            }
        }

        stage('🚀 Deploy') {
            steps {
                echo "Deploying ${env.APP_NAME}..."
                // Simulate deployment
                sh 'echo Deployment done!'
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
