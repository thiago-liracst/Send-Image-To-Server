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
                sh "npm install"
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