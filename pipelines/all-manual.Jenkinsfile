pipeline{
    agent any 
    stages{
        stage('static-analysis'){
            steps{
              echo 'static-analysis'
              script {
                input message: 'have you done ... ?'
                ok: 'Yes, I have.'
              }
            }
        }
        stage('build'){
            steps{
                echo 'build'
            }
        }
        stage('unit tests'){
            steps{
                echo 'unit tests'
            }
        }
        stage('package'){
            steps{
                echo 'package'
            }
        }
    }
}