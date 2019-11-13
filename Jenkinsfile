 pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
            }
        }
        stage('Deploy') {
            steps {
                bat 'xcopy -E ./ C:\\xampp\\htdocs\\'
            }
        }
        stage('cleaning'){
            steps {
                cleanWs()
            }
        }
    }
}