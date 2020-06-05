pipeline {
    agent any
    stages {
        stage("first stage") {
            steps {
                script {
                    sh "ls -al /"
                    def file = readFile "/etc/hosts"
                    echo "Showing file contents..."
                    echo file
                }
            }
        }
    }
}