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
        bat 'C:\\DevOps\\GitRep\\creating-a-pipeline-in-blue-ocean\\jenkins\\scripts\\test.sh'
      }
    }
  }
}