pipeline {
  agent any
  stages {
    stage('check code') {
      steps {
        git(url: 'https://github.com/shaineminkyaw/bank-project', branch: 'master')
      }
    }

    stage('logs') {
      steps {
        sh 'ls -la'
      }
    }

  }
}