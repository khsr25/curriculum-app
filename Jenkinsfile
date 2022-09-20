pipeline {
  agent any
  stages {
    stage('checkout code') {
      steps {
        git(url: 'https://github.com/khsr25/curriculum-app.git', branch: 'dev')
      }
    }

    stage('log') {
      steps {
        sh 'ls -la'
      }
    }

  }
}