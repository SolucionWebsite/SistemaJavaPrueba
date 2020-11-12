pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                sh 'echo "Hello World"'
                git url: 'https://github.com/SolucionWebsite/SistemaJavaPrueba.git'
                def appVersion = version()
                if (appVersion) {
                    echo "Building version ${appVersion}"
            }
        }
    }
}

 
