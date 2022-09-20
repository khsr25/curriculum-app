pipeline {
  agent any
  stages {
    stage('checkout code') {
      steps {
        git(url: 'https://github.com/khsr25/curriculum-app.git', branch: 'dev')
      }
    }

    stage('log') {
      parallel {
        stage('log') {
          steps {
            sh 'ls -la'
          }
        }

        stage('Front-end Unit-test') {
          steps {
            sh 'cd curriculum-front && npm -i && npm run test:unit'
          }
        }

      }
    }

  }
}