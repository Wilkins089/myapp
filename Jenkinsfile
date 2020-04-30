pipeline {
    agent any
    options {
        timeout(time: 5, unit: 'MINUTES')
    }

    stages {
        stage('Pulling Files') {
            steps {
                sh 'rsync -avz /var/lib/jenkins/workspace/myapp/ wortizdev:/home/ubuntu/myapp/'
            }
        }
        stage('Listing Files') {
            steps {
                sshagent(['wortiz']) {
                    sh 'ssh -tt wortizdev ls -l myapp'
                }
            }
        }
    }
}