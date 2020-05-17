pipeline {
    agent any
    options {
        timeout(time: 5, unit: 'MINUTES')
    }

    stages {
        stage('Deploy to development') {
            when {
                expression {
                    return BRANCH == 'development';
                }
            }
            steps {
                sh 'ls -la'
            }
         }
    }
}
