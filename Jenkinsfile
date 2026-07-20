pipeline {
    agent any
    stages {
        stage ("Build") {
            steps {
                sh 'docker build -t karthik621/abinay:train .'
            }
        }
        stage ("Deploy") {
            steps {
                sh 'docker run -itd --name train -p 9999:80 karthik621/abinay:train'
            }
        }
    }
}
