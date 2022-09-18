pipeline {
  agent any
  stages {
    stage('Checkout Code') {
      steps {
        git(url: 'https://github.com/runingcoder/curriculum-app', branch: 'dev')
      }
    }

    stage('Log') {
      parallel {
        stage('Log') {
          steps {
            sh '''ls -al
'''
          }
        }

        stage('Curriculum Fronted -unit test') {
          steps {
            sh 'cd curriculum-front && npm i && npm run unit:test'
          }
        }

      }
    }

  }
}