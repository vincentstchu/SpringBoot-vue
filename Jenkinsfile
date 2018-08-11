pipeline {
  agent {
    node {
      label 'remote node test'
    }
    
  }
  stages {
    stage('build') {
      agent {
        node {
          label 'remote node test'
        }
        
      }
      steps {
        sh 'maven clean install '
        echo 'hello world'
      }
    }
  }
  environment {
    MAVEN_HOME = '/usr/local/maven'
  }
}