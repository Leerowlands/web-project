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
                bat 'xcopy "C:\\Program Files (x86)\\Jenkins\\workspace\\webpage" C:\\xampp\\htdocs\\ /e /s /y' 
            }
        }
        /*stage('cleaning'){
            steps {
                cleanWs()
            }
        }*/
    } 
    post {
        aborted {
            echo "ABORTED"

        }

    success {
        echo "SUCCESS"
        //env.ForEmailPlugin = env.WORKSPACE
        emailext to:'leerowlands30@yahoo.co.uk',
        subject: env.JOB_NAME,
        body: '''${SCRIPT, template="lee.template"}'''
    }   

    failure { 
        echo "FAILURE"
        }
    }
}
  
