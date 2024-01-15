pipeline {
    agent any
     triggers { 
         pollSCM('*/2 * * * *') }
    stages {
        stage('Clone') {
            steps {
                cleanWs()
                bat "git clone https://github.com/relzeid/devops24.git"    
            }
        }
        stage('Build') {
            steps {
                echo 'Hello Build'
                     
            }
        }
        stage('Docker') {
            steps {
               bat 'docker pull hello-world'
               bat 'docker run hello-world'
            }
        }
         stage('Test') {
            steps {
                echo 'Hello Test'
            }
             stage('Python') {
            steps {
                bat 'try.py'
            }
        }
         stage('Deploy') {
            steps {
                echo 'Hello Deploy'
            }
        }
    }
}
