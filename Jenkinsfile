pipeline {
  agent {
    node {
      label 'workstation'
    }
  }
  stages {
    stage('Docker build') {
      steps {
        sh 'docker build -t docker.io/jedkink/rb-frontend .'
      }
    }

    stage('Docker Push') {
      steps {
        sh 'docker push docker.io/jedlink/rb-frontend'
      }
    }

  }
}