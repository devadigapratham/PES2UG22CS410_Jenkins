pipeline {
    agent any 

    stages {
        stage('Build') {
            steps {
                script {
                    sh 'g++ -o output main/main.cpp'
                }
            }
        }

        stage('Test') {
            steps {
                script {
                    sh 'exit 1'
                }
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deployment Successful'
            }
        }
    }

    post {
        failure {
            echo 'Pipeline failed!'
        }
    }
}
