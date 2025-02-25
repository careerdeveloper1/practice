pipeline {
    agent any
    stages {
        stage('isntall nginx') {
            steps {
                sh '''sudo apt-get update
                sudo apt-get install -y nginx
                sudo nginx -v'''
            }
        }
    }
}
