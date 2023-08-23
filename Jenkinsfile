pipeline {
    agent any
    
    tools{
        jdk 'jdk11'
        maven 'maven3'
    }

    stages {
        stage('Git checkout') {
            steps {
                git 'https://github.com/adedokunk/website.git'
            }
        }
        
        stage('Build') {
            steps {
                sh 'mvn clean install package'
            }
        }
    }
}
