pipeline {
  agent any
  stages {
    stage('build') {
      agent any
      steps {
        sh 'maven clean install '
        echo 'hello world'
      }
    }
  }
}