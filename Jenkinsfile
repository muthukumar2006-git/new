pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                // Pulls the latest code from your repository
                checkout scm
            }
        }

        stage('Run Python Script') {
            steps {
                // Runs the Python script on Linux/Mac agents
                sh 'python3 python.py'
                
                // If your Jenkins agent is running on Windows, replace the line above with:
                // bat 'python app.py'
            }
        }
    }
}
