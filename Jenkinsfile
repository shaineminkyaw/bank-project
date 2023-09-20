pipeline {
  agent any
  stages {
    stage('checkout code') {
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