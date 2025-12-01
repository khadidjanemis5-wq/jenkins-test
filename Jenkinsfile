pipeline {
  agent any
  stages {
    stage('Checkout') {
      steps {
        git 'https://github.com/khadidjanemis5-wq/MonApp.git'
      }
    }
    stage('Build Image') {
      steps {
        sh 'docker build -t python-print-app .'
      }
    }
    stage('Run Container') {
      steps {
        sh 'docker run --rm python-print-app'
      }
    }
  }
}