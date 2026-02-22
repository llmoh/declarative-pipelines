pipeline {
    agent any 

    triggers {
        // At 22:00 on every day-of-week from Monday through Friday.
        cron('0 22 * * 1-5')
    }

    stages {
        stage ('SCM') {
            steps {
                git branch: 'main', url: 'https://github.com/llmoh/declarative-pipelines.git'
            }
        }
        stage('build') {
            steps {
               echo 'build the code ...'
            }
        }
        stage('package') {
            when{
                expression {
                    return params.branch = "release"
                }
            }
            steps {
               echo 'packaging the code for release ...'
            }
        }
    }
}