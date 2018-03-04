pipeline {
  agent any
  stages {
    stage('Configure') {
      steps {
        sh './configure'
      }
    }
    stage('Build') {
      steps {
        sh 'make'
      }
    }
  }
}