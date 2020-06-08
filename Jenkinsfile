pipeline {
    agent any
    stages {
        stage("main stage") {
            steps {
                script {
                    load "Jenkinsfile_statements"
                    load "Jenkinsfile_os"
                    load "Jenkinsfile_docker"
                    load "Jenkinsfile_embedded_function"
                    load "Jenkinsfile_function"
                }
            }
        }
    }
}