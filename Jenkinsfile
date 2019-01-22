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

'''
      }
    }
    stage('build') {
      steps {
        sh 'gcc -g -Wall -c main.c -o hello'
      }
    }
    stage('test') {
      steps {
        sh './hello '
      }
    }
    stage('archive ') {
      steps {
        archiveArtifacts 'hello'
      }
    }
  }
}