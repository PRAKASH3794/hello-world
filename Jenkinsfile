pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'build stage'
      }
    }

    stage('test') {
      steps {
        bat 'echo "hello test"'
      }
    }

    stage('deploy') {
      steps {
        bat(script: 'success', returnStatus: true, returnStdout: true)
      }
    }

  }
}