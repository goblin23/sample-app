
pipeline {
  agent any

  stages {
    stage('build') {
      steps {
        withMaven(
        // Maven installation declared in the Jenkins "Global Tool Configuration"
        maven: '3.5.2')
         {
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
