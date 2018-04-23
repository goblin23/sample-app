
pipeline {
  agent {
    any
  }

  stages {
    stage('build') {
      steps {
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
