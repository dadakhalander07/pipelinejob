pipeline {
    agent any 
    stages {
        stage('Build') { 
            steps {
                sh 'echo STAGE 1: this is build stage' 
            }
        }
        stage('Test') { 
            steps {
                 sh 'echo STAGE 2: this is test stage'
            }
        }
        stage('Deploy') { 
            steps {
                 sh 'echo STAGE 3: this is deploy stage'
            }
        }
    }
}
