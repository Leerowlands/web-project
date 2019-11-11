pipeline {
    agent any

    tools {nodejs 'node'}

    stages {
        stage('Install dependencies') {
            steps {
                sh 'npm install'
            }
        }
        stage ('Build node')  {
            steps {
                install 'nodejs'
            }      
        }
        stage ('Test') {
            steps {
                echo 'This is the test stage'
            }
        }
        stage ('Deploy to staging') {
            steps {
                echo 'Nearly there'
            }
        }
        stage ('Deploy to production') {
            steps {
                echo 'Off we go to production!'
            }
        }
    }

}