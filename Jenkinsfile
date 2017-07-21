pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'Building..'
        sh '''npm install;
npm run build;'''
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