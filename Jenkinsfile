pipeline {
  agent any
  stages {
    stage('Building') {
      steps {
        tool(name: 'maven', type: 'maven')
        sh '''cd Calculator
mvn -Dmaven.test.failure.ignore=true clean package'''
      }
    }

  }
}