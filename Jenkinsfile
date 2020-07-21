pipeline {
    agent any
    stages {
        stage('Run Tests') {
            parallel {
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
    }
}
