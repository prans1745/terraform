pipeline {
  agent any
  stages {
    stage('dev') {
      parallel {
        stage('dev1') {
          steps {
            build(job: 'one', quietPeriod: 1, waitForStart: true, wait: true)
          }
        }

        stage('dev2') {
          steps {
            sh 'date'
          }
        }

        stage('dev3') {
          steps {
            s3FindFiles 'testtesttest11'
          }
        }

      }
    }

  }
}