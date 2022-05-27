pipeline {
    agent any
    stages {
        stage('build') {
            steps {
                sh 'echo hello world'
                sh 'mvn clean install -Denforcer.fail=false'
            }
        }
    }
}
