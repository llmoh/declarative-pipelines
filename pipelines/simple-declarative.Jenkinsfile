pipeline {
    agent any 
    environment {
        SENTENCE = "Hello everybody I hope that you're doing well"
    }
    stages {
        stage ('stage 1') {
            steps {
                echo 'Hello this is me'
                script {
                    def words = env.SENTENCE.split(' ')
                    for(word in words){
                        echo word
                    }
                }
            }
        }
    }
}