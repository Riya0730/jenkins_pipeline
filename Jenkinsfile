pipeline {
    agent any
    stages {
        stage('Build Docker Image') {
            steps {
                sh 'docker build -t my-simple-app .'
            }
        }
        stage('Run Container') {
            steps {
                sh 'docker run -d -p 5000:5000 my-simple-app'
            }
        }
    }
}
