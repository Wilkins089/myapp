pipeline {
    agent any
    options {
        timeout(time: 10, unit: 'MINUTES')
    }

    stages {
        stage('Deploy to development') {
            when {
                expression {
                    return env.BRANCH == 'development';
                }
            }
            steps {
                sh 'ls -la'
            }
         }
    }
}
