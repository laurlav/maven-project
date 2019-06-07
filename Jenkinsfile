pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                sh 'mvn clean package'
                sh 'docker build . -t tomcatwebapp:${env.BUILD_ID}'
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
