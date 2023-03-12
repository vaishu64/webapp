pipeline {
    agent any

    environment {
        
        PATH ="$PATH:/opt/apache-maven-3.6.3/bin"
    }

    stages {
        stage('GetCode') {
            steps {
                // Get some code from a GitHub repository
                url: 'https://github.com/vaishu64/webapp.git'
                
            }
        }
        stage('Build') {
            steps {
                sh 'mvn clean package'
            }
        }
    }
}