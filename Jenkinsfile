pipeline {
  agent {
    docker {
      image 'python:3.7.2'
      args '-p 3000:3000'
    }

  }
  stages {
    stage('Build') {
      steps {
        sh 'pip install -r requirements.txt'
      }
    }
  }
}