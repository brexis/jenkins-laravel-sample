pipeline {
    agent {
        docker {
            image 'php:7.0'
        }
    }
    stages {
        stage('Build') {
            steps {
                /**
                 * Install composer
                 */
                sh '''
                    wger https://getcomposer.org/composer.phar
                    php composer.phar self-update
                    php composer.phar install --no-interaction
                '''
            }
        }
    }
}
