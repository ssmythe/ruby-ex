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
        sh '''sh \'\'\'#!/bin/bash -l
rvm use 2.2.1@ruby-ex
bundle install
ruby -c config.ru
\'\'\'
'''
      }
    }
  }
}