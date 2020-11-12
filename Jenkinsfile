pipeline {
    agent any
    stages {
        stage('Consultar') {
            steps {
                echo 'Consultando cambios en el repositorio'
                checkout([$class: 'GitSCM', branches: [[name: '*/master']], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[url: 'https://github.com/SolucionWebsite/SistemaJavaPrueba.git']]])
            }
        }
        stage('Clonar') {
            steps {
                echo 'Clonando repositorio GIT'
                git 'https://github.com/SolucionWebsite/SistemaJavaPrueba.git'
            }
        }
        stage('Test') {
            steps {
                echo 'Testeando sistema con Junit'
                junit 'SistemaJavaPrueba/Junitest.xml'
            }
        }
        stage('Ejecutar') {
            steps {
                echo 'Ejecutando repositorio GIT'
            }
        }
    }
}

 
