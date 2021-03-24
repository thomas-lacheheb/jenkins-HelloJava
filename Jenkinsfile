pipeline {
    agent any
    stages {
        stage('clone') {
            steps {
                git branch: 'main', url: 'https://github.com/thomas-lacheheb/jenkins-HelloJava.git'
            }
        }
        stage('build') {
            steps {
                sh "javac Main.java"
            }
        }
        stage('run') {
            steps {
                sh "java Main"
            }
        }
    }
}
