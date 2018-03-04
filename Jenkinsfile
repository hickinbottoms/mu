pipeline {
  agent any
  stages {
    stage('Autogen') {
      steps {
        sh 'autoreconf -i'
      }
    }
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