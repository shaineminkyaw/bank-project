pipeline {
  agent any
  stages {
    stage('check code') {
      steps {
        git(url: 'https://github.com/shaineminkyaw/bank-project', branch: 'master')
      }
    }

    stage('logs') {
      parallel {
        stage('logs') {
          steps {
            sh 'ls -la'
          }
        }

        stage('build go') {
          steps {
            sh 'go build -o app main.go && ./app'
          }
        }

      }
    }

  }
}