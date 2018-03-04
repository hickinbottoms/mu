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
    stage('Autogen') {
      steps {
        sh './autogen.sh'
      }
    }
  }
}