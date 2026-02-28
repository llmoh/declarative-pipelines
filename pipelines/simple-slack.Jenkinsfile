pipeline {
    agent any 
    stages{
        stage('build'){
            steps {
                echo 'build'
            }
        }
        stage('notify'){
            steps {
                echo 'send notification'
                slackSend channel: 'devops', message: 'build has completed'
            }
        }
    }
}