pipeline {
  agent any
  stages {
    stage('hello') {
      steps {
        sh 'echo Hello, BlueOcean!'
      }
    }
    stage('Ruby Syntax Check') {
      steps {
        sh 'ruby -c config.ru'
      }
    }
  }
}