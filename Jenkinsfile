pipeline {
  agent any
  stages {
    stage('Fluffy Build') {
      steps {
        sh './jenkins/test-all.sh'
      }
    }
    stage('Fluffy Test') {
      steps {
        sh './jenkins/test-all.sh'
      }
    }
    stage('Fluffy Deploy') {
      steps {
        sh './jenkins/test-all.sh'
      }
    }
  }
}