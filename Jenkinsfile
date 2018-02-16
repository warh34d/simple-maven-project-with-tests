pipeline {
  agent any
  stages {
    stage('Test') {
      steps {
        bat 'C:/maven/bin/mvn.cmd test'
        junit 'target/surefire-reports/*.xml'
      }
    }
  }
}