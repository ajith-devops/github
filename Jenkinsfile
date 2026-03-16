pipeline {
    agent any

    stages {

        stage('Build Docker Image') {
            steps {
                sh 'docker build -t ajithkumar14542/devops-demo .'
            }
        }

        stage('Push Docker Image') {
            steps {
                sh 'docker push ajithkumar14542/devops-demo'
            }
        }

        stage('Run Container') {
            steps {
                sh 'docker run -d -p 3000:3000 ajithkumar14542/devops-demo'
            }
        }

    }
}