pipeline {
    agent any
    stages {
        stage('mkdir') {
            steps {
                echo '==>start mkdir'
                sh 'cd docker && mkdir data && chmod 775 data'
            }
        }
        stage('run') {
            steps {
                echo '==>start run'
                sh 'cd docker && docker-compose down && docker-compose up -d'
            }
        }
    }
}