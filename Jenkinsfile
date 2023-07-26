pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                echo "building states"
                sh 'echo $PATH'
                sh 'which node'
                sh 'node -v'
                sh 'npm install'
            }
        }
    }
}