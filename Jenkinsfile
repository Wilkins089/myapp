pipeline {
    agent any
    options {
        timeout(time: 10, unit: 'MINUTES')
    }

    stages {
        stage('Deploy to development') {
            when (BRANCH_NAME == 'development') { 
                
            steps {
                sh 'ls -la'
                
               }
            }
        }
    }
}
