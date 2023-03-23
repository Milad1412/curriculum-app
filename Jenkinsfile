pipeline {
  agent any
  stages {
    stage('Checkout Code') {
      steps {
        git(url: 'https://github.com/Milad1412/curriculum-app', branch: 'dev')
      }
    }

    stage('Front-end unit tests') {
      steps {
        sh 'cd curriculum-app && npm i && npm run test:unit'
      }
    }

  }
}