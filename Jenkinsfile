pipeline {
  agent {
    kubernetes {
      //cloud 'kubernetes'
      containerTemplate {
        name 'node'
        image 'node:14-alpine'
        ttyEnabled true
        command 'cat'
      }
    }
  }
  stages {
    stage('build') {
      steps {
        sh 'npm --version'
      }
    }
  }
}
