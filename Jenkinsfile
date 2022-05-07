pipeline {
    agent any
    stages {
        stage('build') {
            steps {
                sh 'echo Hello World'
                sh 'mvn clean install -Denforcer.fail=false'
            }
        }
    }
}
