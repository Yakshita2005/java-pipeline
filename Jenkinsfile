pipeline {
    agent any
    stages{
         stage('clone') {
            steps {
                git branch: 'main', credentialsId: '905d19a9-43ce-4d24-acac-6dd6c96c2734', url: 'https://github.com/Yakshita2005/java-pipeline.git'
            }
        }
        stage('compile') {
            steps {
                bat'javac hello.java'
            }
        }
    
        stage('run') {
            steps {
                bat'java hello'
            }
        }
    }
}
