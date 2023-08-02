pipeline {
    agent any
    environment {
        // Указываем путь к NVM_DIR для Jenkins
        NVM_DIR = '/var/lib/jenkins/.nvm'
        // Активируем нужную версию Node.js
        PATH = "$NVM_DIR/versions/node/v18.17.0/bin:$PATH"
        WORKSAPCE = "/home/ubuntu/project/elochka/frontend"
    }
    stages {
        stage('install node js') {
            steps {
                echo "install nvm and use node js"
                sh "chmod -R 777 ${env.WORKSPACE}"
                sh 'cd /home/ubuntu/project/elochka/frontend'
                sh 'ls -a'
                sh 'hostname'
            }
        }

        stage('Build') {
            steps {
                echo "building states"
                sh 'node -v'
                sh 'cd /home/ubuntu/project/elochka/frontend'
                sh 'yarn start'
                // Далее можете продолжить со сборкой в Build стадии
            }
        }
    }
}
