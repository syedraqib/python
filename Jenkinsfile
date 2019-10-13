pipeline {
  agent any
  stages {
    stage('interactive') {
      agent any
      steps {
        echo 'start of pipeline'
        input(message: 'Approve?', id: 'id', ok: 'yes')
      }
    }
    stage('execute') {
      steps {
        sh 'echo "hello world"'
      }
    }
  }
}