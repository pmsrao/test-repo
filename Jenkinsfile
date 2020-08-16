pipeline {
  agent {
    docker {
      image 'continuumio/anaconda3'
    }

  }
  stages {
    stage('first stage') {
      steps {
        sh 'python --version'
      }
    }

    stage('second stage') {
      steps {
        sh 'pip --version'
      }
    }

    stage('last stage') {
      steps {
        sh 'sudo pip install mlflow'
      }
    }

  }
}