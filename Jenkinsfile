
pipeline {
  agent any

  stages {
    stage('build') {
      steps {
          withMaven {
            echo 'building package'
            sh 'mvn package'
          }
      }
    }
  }

  post {
    always {
      echo 'done'
    }
  }
}
