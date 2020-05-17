pipeline {
    agent any
    options {
        timeout(time: 5, unit: 'MINUTES')
    }

    stages {
        stage('Deploy to development') {
            when {
                branch 'development'
            }
                steps {
                    sh 'ls -la'
                    sh 'pwd'
                    sh 'hostname'
            }
        }
        stage('Deploy to master') {
            when {
                branch 'master'
            }
                steps {
                    sh 'hostname'
                    sh 'pwd'
                    sh 'ls -la'
            }
        }
    }
}
