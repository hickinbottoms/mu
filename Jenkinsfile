pipeline {
  agent any
  stages {
    stage('Autogen') {
      steps {
        sh './autogen.sh'
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
