pipeline {
    agent any
    environment {
        // Указываем путь к NVM_DIR для Jenkins
        NVM_DIR = '/var/lib/jenkins/.nvm'
        // Активируем нужную версию Node.js
        PATH = "$NVM_DIR/versions/node/v18.17.0/bin:$PATH"
    }
    stages {
        stage('install node js') {
            steps {
                echo "install nvm and use node js"
                sh '/home/ubuntu/project/elochka/frontend'
                sh 'ls -a'
                sh 'hostname'
            }
        }

        stage('Build') {
            steps {
                echo "building states"
                sh 'node -v'
                sh 'npm install'
                // Далее можете продолжить со сборкой в Build стадии
            }
        }
    }
}
