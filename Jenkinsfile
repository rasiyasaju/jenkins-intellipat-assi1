pipeline {
    agent { label 'slave' }

    stages {
        stage('Test') {
            steps {
                sh '''
                echo "Running on agent"
                hostname
                pwd
                '''
            }
        }
    }
}
