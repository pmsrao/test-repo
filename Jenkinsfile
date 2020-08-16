pipeline {
  agent {
    docker {
      image 'node:14-alpine'
    }

  }
  stages {
    stage('first stage') {
      steps {
        sh 'node --version'
      }
    }

    stage('second stage') {
      steps {
        sh 'node --version'
      }
    }

    stage('last stage') {
      steps {
        sh 'echo $HOME'
      }
    }

  }
}