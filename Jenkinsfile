library identifier: 'jenkins-shared-library@main',
        retriever: modernSCM([$class: 'GitSCMSource', remote:'https://github.com/KSingla07/jenkins-shared-library.git'])

pipeline {
  agent any
  stages {
    stage('initialize') {
      steps {
        checkDocker()
        sh 'echo "This is Build Number $BUILD_NUMBER from $DEMO"'
      }
    }

  }
}
