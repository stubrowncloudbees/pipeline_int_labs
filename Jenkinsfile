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
  }
}