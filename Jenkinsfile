pipeline {
  agent {
    docker {
      image 'gcc'
    }

  }
  stages {
    stage('scm') {
      steps {
        echo 'gcc --version'
      }
    }
  }
}