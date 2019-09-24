pipeline {
  agent {
    node {
      label 'LABEL'
    }

  }
  stages {
    stage('Build') {
      parallel {
        stage('Build') {
          steps {
            bat 'echo %NAME%'
          }
        }
        stage('Build2') {
          steps {
            bat 'echo Build2'
          }
        }
      }
    }
    stage('Test') {
      steps {
        bat 'echo Test'
      }
    }
  }
  environment {
    NAME = 'Sidd'
  }
}