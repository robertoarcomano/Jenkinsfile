pipeline {
    agent any
    stages {
        stage("parallel stage") {
            parallel {
                stage('Test On Windows') {
                    steps {
                        echo "Windows"
                    }
                    post {
                        always {
                            echo "final Windows"
                        }
                    }
                }
                stage('Test On Linux') {
                    steps {
                        echo "Linux"
                    }
                    post {
                        always {
                            echo "final Linux"
                        }
                    }
                }
            }
        }
    }
    post {
        always {
            steps {
                script {
                    parallel(running_set)
                }
            }
            post {
                always {
                    echo "finished"
                }
            }


//             script {
//                    load "Jenkinsfile_params"
//                load "Jenkinsfile_parallel"
//                    load "Jenkinsfile_statements"
//                    load "Jenkinsfile_os"
//                    load "Jenkinsfile_docker"
//                    load "Jenkinsfile_embedded_function"
//                    load "Jenkinsfile_function"
//                    load "Jenkinsfile_script"
//                    load "Jenkinsfile_parameters"
//                    load "Jenkinsfile_credentials"
//                    load "Jenkinsfile_email"
//             }
        }
    }
}