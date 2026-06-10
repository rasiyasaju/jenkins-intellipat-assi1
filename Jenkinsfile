pipeline {
    agent { label 'slave' }

    stages {

        stage('Pull Code') {
            steps {
                sh '''
                mkdir -p /home/ubuntu/jenkins/project
                '''
            }
        }

        stage('Show Info') {
            steps {
                sh '''
                echo "Running on:"
                hostname

                echo "Current user:"
                whoami

                echo "Files:"
                ls -la
                '''
            }
        }
    }
}
