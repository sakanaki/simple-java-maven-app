pipeline {
    agent any // 或者是 label 'my-label' 或 none，根據你的需要修改
    stages {
        stage('Build') {
            steps {
                sh 'mvn -B -DskipTests clean package'
            }
        }
    }
}