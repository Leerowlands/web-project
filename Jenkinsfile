pipeline {
    agent any

    stages {
        stage ('Build')  {
            steps {
                sh 'nodejs install'
            }      
        }
        stage('Install dependencies') {
            steps {
                sh 'npm install'
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