pipeline {
    agent any
    stages {
        stage("main stage") {
          steps {
            parallel(
              a: stage("stage1") {
                echo "This is branch a"
              },
              b: stage("stage1") {
                echo "This is branch b"
              }
            )
          }
//             steps {
//                 script {
//                    load "Jenkinsfile_params"
//                    load "Jenkinsfile_parallel"
//                    load "Jenkinsfile_parallel_stages"
//                    load "Jenkinsfile_statements"
//                    load "Jenkinsfile_os"
//                    load "Jenkinsfile_docker"
//                    load "Jenkinsfile_embedded_function"
//                    load "Jenkinsfile_function"
//                    load "Jenkinsfile_script"
//                    load "Jenkinsfile_parameters"
//                    load "Jenkinsfile_credentials"
//                    load "Jenkinsfile_email"
//                 }
//             }
        }
    }
}