pipeline {
    agent any

    tools {
        maven 'Maven3'
    }

    stages {
        stage('Build') {
            steps {
                dir('practical') {
                    bat 'mvn clean compile'
                }
            }
        }

        stage('Test') {
            steps {
                dir('practical') {
                    bat 'mvn test'
                }
            }
        }

        stage('Package') {
            steps {
                dir('practical') {
                    bat 'mvn package'
                }
            }
        }
    }
}
