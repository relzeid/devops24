pipeline {
    agent any
     triggers { 
         pollSCM('* * * * *') }
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
        }
         stage('Deploy') {
            steps {
                echo 'Hello Deploy'
            }
        }
    }
}
