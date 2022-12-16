pipeline {
    agent any
    stages {
        stage('Example Build') {
            
            steps {
                docker run --name 3.8.1-adoptopenjdk-11:V2
                echo 'Hello, Maven'
                sh 'mvn --version'
            }
        }
        stage('Example Test') {
            
            steps {
                docker run --name openjdk:8-jre:V2
                echo 'Hello, JDK'
                sh 'java -version'
            }
        }
    }
}
