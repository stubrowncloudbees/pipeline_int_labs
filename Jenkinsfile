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
      parallel {
        stage('Buzz Test') {
          steps {
            sh '''echo I am a $BUZZ_NAME
'''
          }
        }
        stage('Testing A') {
          steps {
            sh '''sleep 10
echo done'''
          }
        }
      }
    }
  }
  environment {
    BUZZ_NAME = 'Worker Bee'
  }
}