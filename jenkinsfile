pipeline {
    agent any
tools {
        jdk 'jdk11'
    }
stages {
        stage('Cloner le repo') {
            steps {
                git url: 'https://github.com/hayat-24/jenkins-helloworld.git', branch: 'main'
            }
        }
stage('Compilation') {
            steps {
                sh 'javac Main.java'
            }
        }
stage('Exécution') {
            steps {
                sh 'java Main'
            }
        }
    }
post {
        always {
            echo 'Pipeline terminé.'
        }
    }
}
