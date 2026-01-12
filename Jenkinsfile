pipeline {
    agent any { label 'AGENT1' }
    stages {
        stage('BUILD') {
            steps {
                script {
                    sh """
                        echo "hello iam build"
                    """
                }
            }
        }
        stage('TEST') {
            steps {
                script {
                    sh """
                        echo "hello iam test"
                    """
                }
            }
        }
        stage('DEPLOY') {
            steps {
                script {
                    sh """
                        echo "hello iam deploy"
                    """
                }
            }
        }
    }
    post {
        always {
            echo "i will always say hello"
        }
        succes {
            echo "i wll run when the pipeline is success"
        }
        failure {
            echo "i will run when the pipeline is failure"
        }
    }
}