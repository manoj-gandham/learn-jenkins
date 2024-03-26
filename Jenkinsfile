pipeline {
  agent any
  stages {
    stage('Parallel') {
      parallel {

        stage('One') {
          steps {
            sh 'echo One'
          }
        }
        stage('Two') {
          steps {
            sh 'echo Two'
          }
        }
        stage('Three') {
          steps {
            sh 'echo Three'
          }
        }

      }
    }



  }
}