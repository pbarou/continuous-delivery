pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
                sh 'composer install'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
                vendor/bin/phpunit -c module/application/test/
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}
