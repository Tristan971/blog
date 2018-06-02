pipeline {
    agent any

    environment {
        LOCATION = '/var/www/blog'
    }

    stages {
        stage('Checkout new version') {
            steps {
                sh 'cd $LOCATION && git reset --hard origin/master && git pull --force'
            }
        }
    }
}
