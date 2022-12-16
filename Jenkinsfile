pipeline {
    agent any
    stages {
        stage('Example Build') {
            
            steps {
               
                docker run --name Build -d openjdk
                echo 'Hello, Maven'
                sh 'mvn --version'
            }
        }
        stage('Example Test') {
            
            steps {
                docker run --name Test -d openjdk:8-jre
                echo 'Hello, JDK'
                sh 'java -version'
            }
        }
    }
}
