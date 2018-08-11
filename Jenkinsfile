pipeline {
  agent {
    node {
      label 'remote'
    }
    
  }
  stages {
    stage('build') {
      agent {
        node {
          label 'remote'
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