pipeline {
  agent {
    docker {
      image 'frolvlad/alpine-gcc'
    }

  }
  stages {
    stage('scm') {
      steps {
        echo 'hi guys'
        sh '''gcc --version

gcc -g -Wall -c main.c -o hello'''
      }
    }
  }
}