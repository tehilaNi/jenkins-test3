pipeline {
  agent {
    label 'ec2-dynamic'   // <--- use your EC2 label here
  }
  stages {
    stage('Preparation') {
      steps {
        echo 'Starting pipeline on EC2 agent...'
        sh 'hostname'
      }
    }
    stage('Checkout') {
      steps {
        echo 'Listing repo files:'
        sh 'ls -l'
      }
    }
    stage('Build') {
      steps {
        echo 'Simulating build step...'
        sh 'echo "Build step complete"'
      }
    }
    stage('Test') {
      steps {
        echo 'Simulating tests...'
        sh 'echo "All tests passed ✅"'
      }
    }
  }
}

