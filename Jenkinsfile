pipeline {
    agent any // 或者是 label 'my-label' 或 none，根據你的需要修改
    stages {
        stage('Build') {
            agent {
                // 在這裡定義代理類型
                // 如果要在 Docker 容器中運行，可以省略此部分
            }
            steps {
                sh 'mvn -B -DskipTests clean package'
            }
        }
    }
}