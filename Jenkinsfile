pipeline {
    agent any    
    stages {
        stage('build'){
          steps {
            sh 'npm install'
          } 
        }
        stage('unit-tests'){
          steps{
            sh 'npm run unit-test'
          } 
        }
        stage('integration-tests'){
         when{
            anyOf {
                branch 'develop'
                branch 'main'
            }
         }
          steps{
            sh 'npm run integration-test'
          }
       }
       stage('deploying-tests'){
         when{
            branch 'main'
         }
          steps{            
            echo 'Deploying...'
          }
       }                     
    }
}