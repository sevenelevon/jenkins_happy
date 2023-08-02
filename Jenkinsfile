pipeline {
    agent any
    environment {
        // Указываем путь к NVM_DIR для Jenkins
        NVM_DIR = '/home/ubuntu/'
        // Активируем нужную версию Node.js
        PATH = "$NVM_DIR/versions/node/v18.17.0/bin:$PATH"
    }
    stages {
        
        stage('install node js') {
            steps {
                echo "install nvm and use node js"
                // sh 'node -v --user 0 --unsafe-perm true'
                // sh 'export NVM_DIR="$HOME/.nvm"'
                // sh 'source "$NVM_DIR/nvm.sh"'
                // sh 'nvm install 18.17.0' // Установите нужную версию Node.js
                // sh 'nvm use 18.17.0' // Активируйте нужную версию Node.js
                sh '/home/ubuntu/project/elochka/frontend'
                sh 'ls -a'
                sh 'hostname'
                // Далее можете продолжить со сборкой в
            }
        }

        // stage('Build') {

        //     steps {
        //         echo "building states"
        //         sh 'node -v'
        //         sh 'npm install'
        //     }
        // }
    }
}
