pipeline {
  agent any
  stages {
    stage('scm') {
      steps {
        sh '''#!/bin/bash 

echo $pwd

gcc -g -Wall -c hello.c -o hello '''
      }
    }
  }
}