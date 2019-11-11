pipeline {
    agent any
    stages {
        stage ('Build') {
            steps {
                'node js'
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