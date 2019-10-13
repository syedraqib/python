pipeline {
  agent any
  stages {
    stage('print') {
      agent any
      steps {
        echo 'start of pipeline'
      }
    }
    stage('execute') {
      steps {
        sh 'python test.py'
      }
    }
  }
}