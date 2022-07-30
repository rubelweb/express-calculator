pipeline{
    agent any
    stages {
        /* stage('Backend'){
             agent{
                docker { image 'maven:3.8.1-adoptopenjdk-11'} 
             }
             steps{
                echo 'Backend...'
                sh 'mvn --version'
            }
        }
        stage('Frontend'){
            agent{
                 dockerfile true 
             }
             steps{
                echo 'Frontend...'
                sh 'svn --version'
                sh 'node --version'
            }
        } */

        stage('Run npm') {
            steps {
                sh 'npm install'
                sh 'npm run unit-test'
                sh 'npm run integration-test'
            }
        }        
    }
}