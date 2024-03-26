pipeline {

  agent {
    node {
      label 'workstation'
    }
  }

  triggers { pollSCM('H/2 * * * *') }

  options {
          ansiColor('xterm')
  }

  parameters {
          string(name: 'Dev', defaultValue: 'test', description: 'Who should I say hello to?')
  }

  environment {
    url_name = "mdevops333.online"
    role = "DevOps"
  }

  stages {

    stage('One') {
      steps {
        sh 'echo Hello World'
        sh 'echo ${url_name}'
      }
    }

    stage('two') {
       steps {
         sh 'echo position'
         sh 'echo ${role}'
       }
    }

  }

  post {
    always {
      sh 'echo Post CleanUP steps'
    }
  }
}
