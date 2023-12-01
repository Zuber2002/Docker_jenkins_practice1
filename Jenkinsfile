pipeline {
    agent any

    stages {
        stage('Build Docker Image') {
            steps {
                script {
                    dockerImage = docker.build('my-python-app')
                }
            }
        }

        stage('Run Docker Container') {
            steps {
                script {
                    dockerImage.inside {
                        sh 'python app.py'
                    }
                }
            }
        }
    }
}
