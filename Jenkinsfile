pipeline {
    agent none
    stages {
        stage('Build') {
            agent {
                docker {
                    image 'maven:3.9.9-eclipse-temurin-21-alpine'
                    label 'docker'  // Якщо потрібно обрати агент за міткою (не обов'язково)
                }
            }
            steps {
                sh 'mvn --version'
            }
        }
    }
}
