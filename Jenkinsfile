pipeline {
    agent any
    stages {
        stage("first stage") {
            steps {
                script {
//                     def content = readFile "/etc/hosts"
                    sh "cp /etc/hosts /tmp/hosts1"
                    sh "cat /tmp/hosts1"
//                     sh "ls -al"
//                     writeFile file: "temp", text: content
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