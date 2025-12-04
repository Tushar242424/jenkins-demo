
pipeline {
    agent any
    stages {
        stage('Checkout') {
            steps {
                git branch: 'main', url: 'https://github.com/<your-username>/jenkins-demo.git'
            }
        }
        stage('Deploy') {
            steps {
                sh '''
                mkdir -p /var/www/html
                cp index.html /var/www/html/
                '''
            }
        }
    }
}
