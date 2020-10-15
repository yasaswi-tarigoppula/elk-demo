pipeline {
  agent any 
  stages {
    stage('Build') {
      steps {
        sh 'echo "Build Stage"'
        sh 'ansible-playbook -vv build.yaml --ask-become-pass'
      }
     }

    stage('Test') {
      steps {
        sh 'echo "Test Stage"'
      }
     }

    stage('Deploy') {
      steps {
        sh 'ansible-playbook -vv deploy.yaml --ask-become-pass'
      }
     }
}
}

