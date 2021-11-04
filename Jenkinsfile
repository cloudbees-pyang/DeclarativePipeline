pipeline {
  agent any
  stages {
    
    stage('Checkout Scm') {
      steps {
        git branch:'main', url:'https://github.com/cloudbees-pyang/simple-java-maven-app.git'
      }
    }

    stage('Maven Build 0') {
      steps {
        sh 'mvn install'
      }
    }

  }
}
