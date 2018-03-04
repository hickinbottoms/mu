pipeline {
  agent any
  stages {
    stage('Autogen') {
      steps {
        sh 'autoreconf -i'
      }
    }
    stage('Automake') {
      steps {
        sh 'automake --force-missing --add-missing'
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
