pipeline {
  agent any
  stages {
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
      stage('three') {
        steps {
          sh 'echo Three'
        }
      }
    }

  }
}