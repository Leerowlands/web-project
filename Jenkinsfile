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
     
         post {
            aborted {
                echo "ABORTED"

            }

         success {

             echo "SUCCESS"
             emailext to:'lee.rowlands30@yahoo.co.uk',
             subject: env.JOB_NAME,

             body: '''Webproject is running!!'''
            }

            failure { 

                echo "FAILURE"

            }
    }
}
}  
