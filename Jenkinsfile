pipeline {
  agent any
  stages {
    
    stage('Checkout Scm') {
      when {
        beforeAgent true
        branch 'main'
      }
      
      steps {
        git 'https://github.com/cloudbees-pyang/simple-java-maven-app.git'
      }
    }

    stage('Maven Build 0') {
      steps {
        sh 'mvn install'
      }
    }

  }
  triggers {
    pollSCM('*/1 * * * *')
  }
}
