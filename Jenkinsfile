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
      environment {
        MAVEN_HOME = '/usr/local/maven'
        JAVA_HOME = '/usr/java/jdk1.8.0_181-amd64/'
      }
      steps {
        sh 'mvn -DskipTests clean package'
        echo 'hello world'
      }
    }
  }
  environment {
    JMAVEN_HOME = '/usr/local/maven'
  }
}