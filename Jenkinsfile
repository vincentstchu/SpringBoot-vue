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
        git(url: 'https://github.com/vincentstchu/SpringBoot-vue.git', branch: 'master')
      }
    }
  }
}