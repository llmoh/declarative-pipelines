pipeline {
    agent any 
    stages {
        stage ('SCM') {
            steps {
                git branch: 'main', url: 'https://github.com/llmoh/declarative-pipelines.git'
            }
        }
        stage('build') {
            steps{
               echo 'build the code ...'
            }
        }
    }
}