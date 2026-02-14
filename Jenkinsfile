pipeline {
    agent any
    stages {
        stage('Deploy') {
            steps {
                sh '''
                sudo yum install -y httpd
                sudo systemctl start httpd
                sudo cp index.html /var/www/html/
                '''
            }
        }
    }
}
