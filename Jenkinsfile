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
        input {
                         message "Should we continue?"
                         ok "Yes"
                       }
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

    stage('three') {
          when {
            expression {
              CI=false
            }
          }
          steps {
            sh 'env'
          }
        }

      }

  post {
    always {
      sh 'echo Post CleanUP steps'
    }
  }
}

