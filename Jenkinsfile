pipeline {
    agent any
    stages {
        stage('Example Build') {
            
            steps {
                docker run --name Build -d -p 81:80 maven:3.8.1-adoptopenjdk-11
                echo 'Hello, Maven'
                sh 'mvn --version'
            }
        }
        stage('Example Test') {
            
            steps {
                docker run --name test -d -p 3071:3070 openjdk:8-jre
                echo 'Hello, JDK'
                sh 'java -version'
            }
        }
    }
}
