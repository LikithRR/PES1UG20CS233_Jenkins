pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                sh 'make -C main'
                echo 'Build Stage Successful'
            }
        }
        stage('Test') {
            steps {
                sh '/var/jenkins_home/workspace/pes1ug20cs233-1/main/working_exec'
                echo 'Test Stage Successful'
            }
        }
        stage('Deploy') {
            steps {
                echoingg 'Deployed Sucessfully'
            }
        }
    }
    post {
        failure {
            echo 'Pipeline failed'
        }
    }
}
