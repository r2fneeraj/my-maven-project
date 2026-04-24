pipeline {
    agent any

    tools {
        maven 'Maven'
    }

    stages {

        stage('Clone') {
            steps {
                git 'https://github.com/r2fneeraj/my-maven-project.git'
            }
        }

        stage('Build') {
            steps {
                bat 'mvn compile'
            }
        }

        stage('Test') {
            steps {
                bat 'mvn test'
            }
        }

        stage('Package') {
            steps {
                bat 'mvn package'
            }
        }
    }
}
