pipeline {
    agent any

    stages {
         stage('Build') {
            steps {
                script {
                    // Run tests if needed
                    sh 'docker build -t pythonlinux .'
                }
            }
        }

        stage('Run') {
            steps {
                script {
                    // Deploy the Docker image as needed
                    sh 'docker run -i pythonlinux'
                }
            }
        }
    }
}
