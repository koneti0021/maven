pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
              checkout scm
                sh "apt install maven"
                sh "mvn clean install"
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}
