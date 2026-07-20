pipeline {
    agent any
    stages {
        stage ("Build") {
            steps {
                sh 'docker build -t karthik621/abinay:bank .'
            }
        }
        stage ("Deploy") {
            steps {
                sh 'docker run -itd --name bank2 -p 4455:80 karthik/abinay:bank'
            }
        }
    }
}
