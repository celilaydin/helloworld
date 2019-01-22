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
        sh 'gcc -c main.c '
      }
    }
    stage('test') {
      steps {
        sh 'chmod +x main '
        sh './main '
      }
    }
    stage('archive ') {
      steps {
        archiveArtifacts 'hello'
      }
    }
  }
}