pipeline {
  agent any
  stages {
    stage('Test') {
      steps {
        bat 'C:/maven/bin/mvn.cmd test -Dmaven.test.failure.ignore=true'
        junit 'target/surefire-reports/*.xml'
      }
    }
    stage('Install') {
      steps {
        bat 'C:/maven/bin/mvn.cmd install'
      }
    }
  }
}