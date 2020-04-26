pipeline {
    agent any
    stages {
        stage('listing files') {
            when{
                branch 'master'
            }
            steps {
              sh 'ls'
           }
        }  
    }
}
