pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'Building..'
        sh '''bat npm --version
bat npm install'''
      }
    }
    stage('Test') {
      steps {
        echo 'Testing..'
        sh 'jest bill_confirmed.spec'
      }
    }
    stage('Deploy') {
      steps {
        echo 'Deploying....'
      }
    }
  }
}