pipeline {
  agent any
  stages {
    stage('initialize') {
      steps {
        sh 'echo "This is Build Number $BUILD_NUMBER from $DEMO"'
      }
    }

  }
  environment {
    DEMO = '1'
  }
}