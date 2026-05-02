pipeline {
    agent any

    stages {
        stage('Build Docker Image') {
            steps {
                sh 'docker build -t prachi/devops-app .'
            }
        }

        stage('Run Container') {
            steps {
                sh 'docker run -d -p 5001:5000 prachi/devops-app'
            }
        }
    }
}
