pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                sh 'g++ temp.cpp -o temp'
                 build job: 'PES1UG20CS231-1', wait: false
                 echo 'Build by CS231 successful'
            }
        }

        stage('Test') {
            steps {
                sh 'cat temp44.cpp'
                echo 'Test by CS231 successful'
            }
        }

        stage('Deploy') {
            steps {
               
                echo 'Deploy by CS231 successful'
            }
        }
    }

    post {
        failure {
            
                echo 'Pipeline Failed'
          
        }
    }
}
