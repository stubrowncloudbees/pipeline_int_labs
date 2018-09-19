pipeline {
  agent any
  stages {
    stage('Buzz Buzz') {
      steps {
        echo 'Beez Buzz'
        sh './jenkins/test-all.sh'
        archiveArtifacts(artifacts: 'jenkins/*.sh', fingerprint: true)
      }
    }
    stage('Buzz Test') {
      steps {
        sh '''echo I am a $BUZZ_NAME
'''
      }
    }
  }
  environment {
    BUZZ_NAME = 'Worker Bee'
  }
}