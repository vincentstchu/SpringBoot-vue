pipeline {
  agent any
  stages {
    stage('checkout source code') {
      agent {
        node {
          label 'fefdora28'
        }
        
      }
      steps {
        sh 'maven clean install '
      }
    }
  }
}