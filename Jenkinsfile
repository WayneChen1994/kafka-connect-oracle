pipeline {
  agent any
  stages {
    stage('Source') {
      steps {
        git 'https://github.com/WayneChen1994/kafka-connect-oracle'
      }
    }

    stage('Build') {
      steps {
        tool 'maven3.6.3'
        sh 'mvn clean package'
      }
    }

  }
  environment {
    COMPLETED_MSG = 'Build done!'
  }
}