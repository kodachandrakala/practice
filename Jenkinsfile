pipeline {
    agent { docker 'kodachandrakala/nanoimg' } 
    stages {
        stage('Example Build') {
            steps {
                sh 'mvn -B clean verify'
            }
        }
    }
}
