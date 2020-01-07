pipeline {
  agent any
  stages {
    stage('Source') {
      steps {
        git(url: 'http://192.168.128.133/root/cobra-jenkins-demo.git', branch: 'master')
      }
    }

  }
  environment {
    COMPLETED_MSG = 'build node'
  }
}