pipeline{
    agent none    
    stages {
        stages('Build'){
          steps{
            npm install
          } 
        }
        stages('Unit-test'){
          steps{
            npm run unit-test
          } 
        }
        stages('Build'){
          steps{
            npm run integration-test
          }
       }                
    }
}