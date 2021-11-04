pipeline {
  agent any
  stages {
    
    stage('Checkout Scm') {
      steps {
        git branch:'main', url:'https://github.com/cloudbees-pyang/simple-java-maven-app.git'
      }
    }

    stage('Building...') {
      steps {
        sh 'echo building...'
      }
    }

    stage('Deploying...') {
      steps {
        sh 'echo deploying...'
      }
    }
  }
}
