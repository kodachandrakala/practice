pipeline {
    agent any
    stages {
        stage('Example Build') {
            
            steps {
                docker 'maven:3.8.1-adoptopenjdk-11'
                echo 'Hello, Maven'
                sh 'mvn --version'
            }
        }
        stage('Example Test') {
            
            steps {
                docker 'openjdk:8-jre'
                echo 'Hello, JDK'
                sh 'java -version'
            }
        }
    }
}
