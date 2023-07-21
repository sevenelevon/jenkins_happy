pipeline {
    agent none // Используйте none, чтобы не использовать агента по умолчанию

    stages {
        stage('Build') {
            agent {
                node { // Добавьте node блок вокруг шагов, которые требуют агента
                    label 'master' // Можно указать метку, но она будет проигнорирована при использовании node без параметров
                }
            }
            steps {
                echo 'Building...'
                sh 'npm install'
            }
        }
        stage('Test') {
            agent {
                node { // Добавьте node блок вокруг шагов, которые требуют агента
                    label 'master' // Можно указать метку, но она будет проигнорирована при использовании node без параметров
                }
            }
            steps {
                echo 'Testing...'
                sh 'npm test'
            }
        }
    }
}
