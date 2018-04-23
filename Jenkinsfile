pipeline {
  agent any
  stages {
    stage('hello') {
      parallel {
        stage('hello') {
          steps {
            sh 'echo Hello, BlueOcean!'
          }
        }
        stage('hello parallel') {
          steps {
            sh 'echo parallel'
          }
        }
      }
    }
    stage('Build Hello') {
      steps {
        build 'hello build job'
      }
    }
  }
}