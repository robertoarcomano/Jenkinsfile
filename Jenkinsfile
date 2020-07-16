pipeline {
    agent any
    stages {
        stage("main stage") {
            steps {
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
                script {
//                    load "Jenkinsfile_params"
                   load "Jenkinsfile_parallel"
//                    load "Jenkinsfile_statements"
//                    load "Jenkinsfile_os"
//                    load "Jenkinsfile_docker"
//                    load "Jenkinsfile_embedded_function"
//                    load "Jenkinsfile_function"
//                    load "Jenkinsfile_script"
//                    load "Jenkinsfile_parameters"
//                    load "Jenkinsfile_credentials"
//                    load "Jenkinsfile_email"
                }
            }
        }
    }
}