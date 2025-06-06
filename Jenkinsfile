pipeline {
    agent {
        docker { image 'maven:3.9.6-eclipse-temurin-21' }
    }
    stages {
        stage('Build') {
            steps {
                export HOME=/var/jenkins_home
                sh 'mvn -B -DskipTests clean package'
            }
        }
    }
}