pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
                sh "cd server & npm test"
            }
        }
        stage('Deploy') {
            agente {
                docker { image 'node'}
            }
            steps {
                echo 'Deploying....'
                sh "git checkout develop"
            }
        }
    }
}