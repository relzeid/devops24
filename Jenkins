pipeline {
    agent any

    stages {
        stage('Clone') {
            steps {
                cleanWs()
                bat "git clone https://github.com/relzeid/devops24"    
            }
        }
        stage('Build') {
            steps {
                echo 'Hello Build'
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
