pipeline{
    agent none    
    stages {
        stage('Build'){
          steps{
            npm install
          } 
        }
        stage('Unit-test'){
          steps{
            npm run unit-test
          } 
        }
        stage('Build'){
          steps{
            npm run integration-test
          }
       }                
    }
}