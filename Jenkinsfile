pipeline {
    agent any
    options {
        timeout(time: 10, unit: 'MINUTES')
    }

    stages {
        stage('Deploy to development') {
            when {
                expression {  env.BRANCH == 'development' }
            }
            steps {
                sh 'ls -la'
            }
         }
    }
}
