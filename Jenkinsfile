pipeline {
  agent any
  stages {
    stage('check') {
      steps {
        git(url: 'https://github.com/waladevops/wala', branch: 'master')
      }
    }

    stage('Log') {
      parallel {
        stage('Log') {
          steps {
            sh '''ls -la
'''
          }
        }

        stage('Front-End Unit Test') {
          steps {
            sh 'cd curriculum-front && npm i && npm  run test:unit'
          }
        }

      }
    }

  }
}