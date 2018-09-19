pipeline {
  agent any
  stages {
    stage('Buzz Buzz') {
      steps {
        echo 'Beez Buzz'
        sh './jenkins/test-all.sh'
        archiveArtifacts(artifacts: 'jenkins/*.sh', fingerprint: true)
        sh '''echo I am a $BUZZ_NAME
./jenkins/build.sh'''
      }
    }
  }
  environment {
    BUZZ_NAME = 'Worker Bee'
  }
}