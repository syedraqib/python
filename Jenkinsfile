pipeline {
  agent any
  stages {
    stage('interactive') {
      agent any
      steps {
        echo 'start of pipeline'
        input(message: 'Approve?', id: 'yes', ok: 'no')
      }
    }
    stage('execute') {
      steps {
        sh 'echo "hello world"'
      }
    }
  }
}