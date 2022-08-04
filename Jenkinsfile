pipeline{
    agent none    
    stages {
        stage('Build'){
          steps{
            sh 'npm install'
          } 
        }
        stage('Unit-test'){
          steps{
            sh 'npm run unit-test'
          } 
        }
        stage('Build'){
          steps{
            sh 'npm run integration-test'
          }
       }                
    }
}