pipeline {
    agent any
tools {
                maven 'M2_HOME'
            }
    stages {
        stage('build') {
            steps {
                sh 'mvn clean'
                sh 'mvn install'
                sh 'mvn package'
              sleep 10
            }
        }
        stage('test') {
            steps {
                sh 'mvn test'
            }
        }
        stage('deploy') {
            steps {
                echo 'deploy step'
              sleep 10
            }
        }
        stage('docker') {
            steps {
                echo 'image step'
            }
        }
    }
}

