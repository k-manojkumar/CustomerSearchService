pipeline {
    agent any

    environment {
     HOME = '.'
     CI = 'true'
 }
    stages {
        stage('Build') {
            steps {
                sh 'npm install'

            }
        }

        stage('Deliver') {
            steps {
                sh 'npm run setup'
                sh 'npm start'

            }
        }
    }
}
