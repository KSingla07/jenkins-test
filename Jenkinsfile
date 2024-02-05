pipeline {
  agent any
  stages {
    stage('initialize') {
      steps {
        echo 'This is Build Number $BUILD_NUMBER of Job $DEMO'
      }
    }

  }
  environment {
    DEMO = '1'
  }
}