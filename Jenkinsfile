pipeline {
    agent any

    stages {
        stage ('Build')  {
            steps {
                bat 'node server.js'
            }      
        }
        stage('Install dependencies') {
            steps {
                bat 'npm install'
            }
        }
        
    }

}