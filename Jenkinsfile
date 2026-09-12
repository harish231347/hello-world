pipeline {
    agent any

    stages {

        stage('Build') {
            steps {
                echo 'Building branch: ' + env.BRANCH_NAME
            }
        }

        stage('Test') {
            steps {
                echo 'Testing branch: ' + env.BRANCH_NAME
            }
        }
    }

    post {
        success {
            echo 'Pipeline successful for branch: ' + env.BRANCH_NAME
        }

        failure {
            echo 'Pipeline failed for branch: ' + env.BRANCH_NAME
        }
    }
}
