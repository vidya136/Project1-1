pipeline {
  agent { docker { image 'python:3.7.2' } }
  stages {
    stage('build') {
      steps {
        bat 'pip install -r requirements.txt'
      }
    }
    stage('test') {
      steps {
        bat 'python test.py'
      }
    }
  }
}
