pipeline {
    agent any
    stages {
        stage("first stage") {
            steps {
                script {
                    load "Jenkinsfile_os"
                    load "Jenkinsfile_docker"
                }

//                     sh "cp /etc/hosts /tmp/hosts1"
//                     sh "cat /tmp/hosts1"
//
//                     def content = readFile "/etc/hosts"
//                     dir ("/tmp") {
//                         writeFile file: "hosts2", text: content
//                     }
//                     def content1 = readFile "/tmp/hosts2"
//                     echo content1
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