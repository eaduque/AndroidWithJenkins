pipeline {
  agent any
  stages {
    stage('clean') {
      steps {
        sh './gradlew clean'
      }
    }
    stage('App Module Test') {
      steps {
        sh './gradlew app:testDebugUnitTest'
      }
    }
  }
}
