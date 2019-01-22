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

'''
      }
    }
    stage('build') {
      steps {
        sh '''gcc -o hello main.c 
ls -la '''
      }
    }
    stage('test') {
      steps {
        sh 'chmod +x hello '
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