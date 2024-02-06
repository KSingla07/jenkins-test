library identifier: 'jenkins-shared-library@main',
        retriever: modernSCM([$class: 'GitSCMSource', remote:'https://github.com/KSingla07/jenkins-shared-library.git'])

pipeline {
  agent any
  stages {
    stage('initialize') {
      steps {
        checkDocker()
        script{
        customLog.info "Karan"
        }
        sh 'echo "This is Build Number $BUILD_NUMBER from $DEMO"'
      }
    }
    stage('dotnet'){
     agent{
        docker {
            image "mcr.microsoft.com/dotnet/sdk:8.0"
        }
     }
     steps{
        sh '''
            dotnet --list-sdks
            dotnet --list-runtimes
        '''
     }
    }

  }
}
