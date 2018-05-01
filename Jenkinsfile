pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh 'chmod 777 gradlew'
        sh '/home/gradle-4.7/bin/gradle build'
      }
    }
    stage('Run') {
      steps {
        sh 'java -jar ./build/libs/ocean-1.0-SNAPSHOT.jar'
      }
    }
  }
}