pipeline {
  agent any
  stages {
    stage('checkout code') {
      steps {
        git(url: 'https://github.com/khsr25/curriculum-app.git', branch: 'dev')
        git(url: 'https://github.com/khsr25/curriculum-app.git', branch: 'dev')
      }
    }

    stage('Log') {
      parallel {
        stage('Log') {
          steps {
            sh 'ls -la'
          }
        }

        stage('front-end unit-test') {
          steps {
            sh 'cd curriculum-app && npm i && npm run test:unit'
          }
        }

      }
    }

  }
}