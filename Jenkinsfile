pipeline {
  agent any 
  stages {
    stage('Build') {
      steps {
        sh 'echo "Build Stage"'
      }
     }

    stage('Test') {
      steps {
        sh 'echo "Test Stage"'
      }
     }

    stage('Deploy') {
      steps {
        sh 'ansible-playbook -vvvv main.yaml --ask-become-pass'
      }
     }
}
}

