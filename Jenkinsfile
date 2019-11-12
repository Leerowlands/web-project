pipeline {
  agent any
    
  tools {nodejs "server"}
    
  stages {
    stage('Build') {
      steps {
        sh 'nodejs install'
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