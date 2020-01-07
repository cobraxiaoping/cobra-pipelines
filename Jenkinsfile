pipeline {
  agent any
  stages {
    stage('Source') {
      steps {
        git(url: 'http://192.168.128.133/root/cobra-jenkins-demo.git', branch: 'master')
      }
    }

    stage('Build') {
      steps {
        tool 'apache-maven-3.6.1'
        sh 'mvn -v'
      }
    }

  }
  environment {
    COMPLETED_MSG = 'build node'
  }
}