pipeline {
    agent any

    stages {
        stage ('Build')  {
            steps {
                sh 'node server.js'
            }      
        }
        stage('Install dependencies') {
            steps {
                sh 'npm install'
            }
        }
        
    }

}