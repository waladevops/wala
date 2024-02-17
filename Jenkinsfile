pipeline {
  agent any
  stages {
    stage('check') {
      steps {
        git(url: 'https://github.com/waladevops/wala', branch: 'master')
      }
    }

    stage('Log') {
      steps {
        sh '''ls -la
'''
      }
    }

  }
}