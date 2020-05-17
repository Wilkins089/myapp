pipeline {
    agent any
    options {
        timeout(time: 5, unit: 'MINUTES')
    }

    stages {
        stage('Simple echo') {
            steps {
                echo 'Hello people from the GALAXY'
            }
        }

        stage('Deploy to development') {
            when {
                branch 'origin/development'
            }
            steps {
                sh 'ls'
            }
        }
    }
}
