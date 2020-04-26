pipeline {
    agent any

    stages {
        stage('Deploy') {
            branch "master"
            when {env.BRANCH == "master"}
            steps {
                echo 'Deploying....'
            }
        }
    }
}
