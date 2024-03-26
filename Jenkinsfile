pipeline {
 agent any
    stages {
    parallel {
        stage ('one') {
            step {
                sh 'echo hey'
            }
        }
        stage ('two') {
              step {
                sh 'echo hai'
             }
        }
        stage ('three') {
              step {
                 sh 'echo hello'
              }
        }


    }

    }

}