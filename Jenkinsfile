pipeline {
    agent { label 'slave' }

    stages {

        stage('Checkout Source') {
            steps {
                checkout scm
            }
        }

        stage('Copy To Folder') {
            steps {
                sh '''
                mkdir -p /home/ubuntu/jenkins/project

                cp -r * /home/ubuntu/jenkins/project/

                echo "Contents of deployment folder:"
                ls -la /home/ubuntu/jenkins/project
                '''
            }
        }
    }
}
