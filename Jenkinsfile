pipeline {
    agent any
    stages {
       
        stage('Build Docker Image') {
            steps {
                bat 'docker build -t first:v1 .'
            }
        }
        stage('Run Docker Container') {
            steps {
                bat 'docker run -d --name firstapp first:v1'
            }
        }
    }
}
