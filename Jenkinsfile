pipeline {
    agent any
    stages {
        stage("first stage") {
            steps {
                script {
                    def content = readFile "/etc/hosts"
                    sh "cp /etc/hosts ."
                    echo pwd tmp:false
                    sh "ls -al"
                    writeFile file: "temp", text: content
                }
//                 script {
//                     sh "ls -al /"
//                     def file = readFile "/etc/hosts"
//                     echo "Showing file contents..."
//                     echo file
//                     load "secondJenkinsfile"
//                 }
            }
        }
    }
}