library 'SharedLibs'
pipeline {
  agent any
  stages {
    stage('Say Hello') {
      steps {
        echo "Hello ${MY_NAME}!"
      }
    }
    stage('Shared Lib') {
         steps {
             helloWorld("Jenkins")
         }
      }
  }
  environment {
    MY_NAME = 'Daniel'
  }
  post {
    aborted {
      echo 'Why didn\'t you push my button?'
      
    }
    
  }
  parameters {
    string(name: 'Name', defaultValue: 'whoever you are', description: 'Who should I say hi to?')
  }
}
