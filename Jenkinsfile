pipeline {
    agent any
    stages {
        stage("main stage") {
            steps {
                script {
                    load "Jenkinsfile_os"
                    load "Jenkinsfile_docker"
                }
            }
        }
    }
}