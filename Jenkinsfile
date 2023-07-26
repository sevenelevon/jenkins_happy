pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                echo "install nvm and use node js"
                sh 'export NVM_DIR="$HOME/.nvm"'
                sh 'source "$NVM_DIR/nvm.sh"'
                sh 'nvm install 18.17.0' // Установите нужную версию Node.js
                sh 'nvm use 18.17.0' // Активируйте нужную версию Node.js
                // Далее можете продолжить со сборкой в
            }

            steps {
                echo "building states"
                sh 'node -v'
                sh 'npm install'
            }
        }
    }
}