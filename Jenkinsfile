pipeline {
  agent any
  stages {
    stage('Source') {
      steps {
        git 'https://github.com/WayneChen1994/kafka-connect-oracle'
      }
    }

  }
  environment {
    COMPLETED_MSG = 'Build done!'
  }
}