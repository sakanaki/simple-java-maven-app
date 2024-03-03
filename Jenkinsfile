pipeline {
    agent {
        docker {
            image 'maven:3.9.3-eclipse-temurin-17'
            label 'my-defined-label'
            args  '-v /tmp:/tmp'
        }
    }
    options {
        // Timeout counter starts AFTER agent is allocated
        timeout(time: 1, unit: 'SECONDS')
    }
    stages {
        stage('Example') {
            steps {
                echo 'Hello World'
            }
        }
    }
}