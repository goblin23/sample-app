
pipeline {
  agent any

  stages {
    stage('build') {
      withMaven {
        echo 'building package'
        sh 'mvn package'
      }
    }
  }

  post {
    always {
      echo 'done'
    }
  }
}
