pipeline {
    agent {
        docker {
            image 'php:7.0'
        }
    }
    stages {
        stage('Build') {
            steps {
                sh 'composer self-update'
                sh 'composer install --no-interaction'
            }
        }
    }
}
