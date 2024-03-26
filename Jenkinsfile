pipeline {
    agent {
        node {
        label 'workstation'
        }
    }

    environment{
        url = "mdevops333.online"

    }

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
                echo '${var.url}'
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