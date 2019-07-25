pipeline {
  agent {
    label 'docker'
  }
  stages {
    stage('build') {
        agent { docker { image 'python:3.7.2' } }
         steps {
            bat 'pip install -r requirements.txt'
               }
    }
    stage('test') {
        agent { docker { image 'python:3.7.2' } }
        steps {
        bat 'python test.py'
              }
    }
  }
}
