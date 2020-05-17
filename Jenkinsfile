pipeline {
    agent any
    options {
        timeout(time: 5, unit: 'MINUTES')
    }

    stages {
        stage('Deploy to development') {
            when {
                expression {env.BRANCH == 'origin/development'}
            }
            steps {
                sh 'ls -la'
            }
         }
    }
}
