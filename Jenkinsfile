pipeline {
  agent {
    docker {
      image 'gcc'
    }

  }
  stages {
    stage('scm') {
      steps {
        echo 'hi guys'
        sh '''gcc --version


pwd 

ls '''
      }
    }
  }
}