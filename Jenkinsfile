pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                git 'https://github.com/SolucionWebsite/SistemaJavaPrueba.git'
            }
        }
        stage('Build') {
            steps {
                echo 'Building..'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}

 
