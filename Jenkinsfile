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
            steps {
                echo 'Deploying....'
                sh "git checkout develop"
            }
        }
    }
}