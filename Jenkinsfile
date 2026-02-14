pipeline {
    agent any

    stages {

        stage('Build') {
            steps {
                echo "Hello Vandana DevOps World!"
            }
        }

        stage('Deploy') {
            steps {
                sh '''
                sudo apt update
                sudo apt install -y apache2
                sudo systemctl start apache2
                sudo cp index.html /var/www/html/
                '''
            }
        }

    }
}
