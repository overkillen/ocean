pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh '$GRADLE_HOME build'
      }
    }
    stage('Run') {
      steps {
        sh 'java -jar ./build/libs/ocean-1.0-SNAPSHOT.jar'
      }
    }
  }
}