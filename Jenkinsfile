pipeline {
    agent any
    stages {
        stage("first stage") {
            steps {
                sh "ls -al /"
                readFile "/etc/hosts"
            }
        }
    }
}