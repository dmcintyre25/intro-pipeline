pipeline {
  agent any
  stages {
    stage('Say Hello') {
      steps {
        echo "Hello ${NODE_NAME}!"
      }
    }
  }
  environment {
    MY_NAME = 'Daniel'
  }
}