pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
            }
        }
        stage('Test') {
            agent {
                docker {image 'node'}
            }
            steps {
                echo 'Testing..'
                sh 'npm -v'
            }
        }
        stage('Homolação') {
            steps{
                echo 'Promovendo para homolagação'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}
