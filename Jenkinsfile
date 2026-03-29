pipeline {
    agent any

    stages {

        stage('Build Artifact') {
            steps {
                echo 'Building using Maven'
                sh 'mvn clean install'
            }
        }

        stage('Build Docker Image') {
            steps {
                echo 'Building Docker Image'
                sh 'docker build -t teja1612fr/devops-app .'
            }
        }

        stage('Push Docker Image') {
            steps {
                echo 'Pushing Docker Image'
                withCredentials([usernamePassword(credentialsId: 'docker-cred', usernameVariable: 'USER', passwordVariable: 'PASS')]) {
                    sh '''
echo $PASS | docker login -u teja1612fr --password-stdin
'''
                    sh 'docker push teja1612fr/devops-app'
                }
            }
        }

    }
}
