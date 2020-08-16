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
        sh 'conda --version'
        sh 'conda create --name env_mlflow python=3.7'
        sh 'conda activate env_mlflow'
        sh 'pip install mlflow'
      }
    }

  }
}