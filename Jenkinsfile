pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        bat 'npm install'
      }
    }
    stage('Test') {
      agent any
      environment {
        CI = 'true'
      }
      steps {
        bat 'jenkins/scripts/test.sh'
      }
    }
  }
}