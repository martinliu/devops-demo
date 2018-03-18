pipeline {
  agent any
  stages {
    stage('build') {
      parallel {
        stage('build') {
          steps {
            sh 'echo \'hello, world!\''
          }
        }
        stage('test') {
          steps {
            echo 'hello world'
          }
        }
      }
    }
    stage('ship') {
      steps {
        echo 'ship to registratry'
      }
    }
    stage('run') {
      steps {
        echo 'Run docker'
      }
    }
  }
}