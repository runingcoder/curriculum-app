pipeline {
  agent any
  stages {
    stage('Checkout Code') {
      steps {
        git(url: 'https://github.com/runingcoder/curriculum-app', branch: 'dev')
      }
    }

    stage('Log') {
      steps {
        sh '''ls -al
'''
      }
    }

  }
}