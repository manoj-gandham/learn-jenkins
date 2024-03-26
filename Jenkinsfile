pipeline {

  agent {
    node {
      label 'workstation'
    }
  }

  environment {
    url_name = "mdevops333.online"
  }

  stages {

    stage('One') {
      steps {
        sh 'echo Hello World'
        sh 'echo ${url_name}'
      }
    }

  }

  post {
    always {
      sh 'echo Post CleanUP steps'
    }
  }

}