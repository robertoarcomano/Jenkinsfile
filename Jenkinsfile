pipeline {
    agent any
    stages {
        stage("first stage") {
            steps {
                sh "ls -al /"
                def file = readFile "/etc/hosts"
                echo file
            }
        }
    }
}