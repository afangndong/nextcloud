pipeline {
  agent any
  stages {
    stage('Checkout') {
      steps {
        git 'https://github.com/afangndong/nextcloud-k8s.git'
      }
    }

    stage('Deploy to Minikube') {
      steps {
        bat 'kubectl apply -f kubernetes/'
      }
    }
  }
}
