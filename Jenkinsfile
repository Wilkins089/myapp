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
            expression {
                echo "BRANCH_NAME is ${env.BRANCH_NAME}"
                return env.BRANCH_NAME == "development"

                steps {
                    echo 'Hello people from RD'
                }
            }
        }
    }
}
