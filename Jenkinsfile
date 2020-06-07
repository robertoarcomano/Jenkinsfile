pipeline {
    agent any
    stages {
        stage("first stage") {
            steps {
                script {
                    def content1 = readFile "/etc/hosts"
                    dir ("temporary") {
                        writeFile file: "hosts_new", text: content1
                        sh "pwd"
                        sh "ls -al"
                        sh "cat hosts_new"
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