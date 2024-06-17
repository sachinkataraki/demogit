pipeline {
    agent any

    stages {
        stage('Clone source code') {
            steps {
               git credentialsId: 'CICDkey', url: 'https://github.com/akramdevopstrainer/maven-standalone-application.git'
            }
        }
        stage('Software Build using maven'){
            steps {
                echo 'Building using maven'
            }
            
        }
        stage('Testing using Sonarqube'){
            steps {
                echo 'Testing using Sonarqube'
            }
        }
        stage('Deploy using Ansible'){
            steps {
                echo 'Deploying using Ansible'
            }
        }
        stage('Send Confirmation email'){
            steps {
                echo 'Sending Confirmation email'
            }
        }
    }
}
