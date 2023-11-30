pipeline {
    agent any
    
    stages {
        stage('build') {
            steps {
                // Set up a virtual environment
                sh 'python3 -m venv venv'
                
                // Activate the virtual environment
                sh 'source venv/bin/activate'

                // Install dependencies (if you have a requirements.txt file)
                sh 'pip install -r requirements.txt'

                // Run your Python script
                sh 'app.py'
            }
        }
    }
}
