pipeline {
  agent any
  stages {
    
    stage('Checkout Scm') {
      steps {
        git branch:'main', url:'https://github.com/cloudbees-pyang/simple-java-maven-app.git'
      }
    }

    stage('Build') {
      steps {
        sh 'echo building...'
      }
    }

    stage('Test') {
      steps {
        sh 'echo testing...'
      }
    }
  }
}
