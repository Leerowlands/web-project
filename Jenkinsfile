pipeline {
  agent any
    
  tools {nodejs "server"}
    
  stages {
    stage('Build') {
      steps {
        sh 'npm start'
      }
    }
        
    stage('Install dependencies') {
      steps {
        sh 'npm install'
      }
    }
     
    stage('Test') {
      steps {
         sh 'npm test'
      }
    }      
  }
}