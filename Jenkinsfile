pipeline{
    agent none    
    stages {
        stages('Build'){
          steps{
            sh 'npm install'
          } 
        }
        stages('Unit-test'){
          steps{
            sh 'npm run unit-test'
          } 
        }
        stages('Build'){
          steps{
            sh 'npm run integration-test'
          }
       }                
    }
}