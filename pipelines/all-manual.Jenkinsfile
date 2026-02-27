pipeline{
    agent any 
    stages{
        stage('static-analysis'){
            steps{
              echo 'static-analysis'
              script {
                def number = input (
                    message: 'have you performed static analysis and ... ?',
                    parameters: [
                        string(name : 'Value', description : 'Enter a value equally divisibled by 3')
                    ]
                )

                def num = number.toInteger()

                if(num%3 == 0){
                   echo 'divisible by 3'
                } else {
                    error 'not divisibled by 3'
                }
                
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