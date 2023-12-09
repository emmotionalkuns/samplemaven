pipeline {
    agent any
    tools {
        maven 'maven17'
    } 
   stages {
        stage('Git Checkout') {
            steps {
                checkout([$class: 'GitSCM', branches: [[name: '*/main']], extensions: [], userRemoteConfigs: [[url: 'https://github.com/emmotionalkuns/my-jenkins.git']]])
            }
        }
        stage('Build') {
            steps {
                sh 'mvn clean install'
            }
        }
   }
}
