pipeline{
    agent {
        docker { image 'node:14-alpine' }
    }
    stages {
        stage('Build'){
             environment {
                  HOME="."
                }
            steps{
                echo 'Building...'
                sh 'node --version'
            }
        }
        stage('Test'){
             environment {
                  HOME="."
                }
            steps{
                echo 'Testing...'
                sh 'node --version'
            }
        }
        stage('Deploy'){
             environment {
                  HOME="."
                }
            steps{
                echo 'Deploy...'
                sh 'node --version'
            }
        }
    }
}
