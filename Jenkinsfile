pipeline {
    agent any
    stages {
        stage('Install dependencies') { 
            steps {
                bat 'npm install' 
                
            }
        }
        stage('Build'){
          steps{
            'npm run node.js'
          }
        }
        
    }  
}   