pipeline {
  agent any
  stages {
    stage('Clone repo') {
      steps {
        git 'https://github.com/overkillen/ocean.git'
      }
    }
    stage('Build') {
      steps {
		sh 'chmod 777 gradlew'
        sh './gradlew build'
      }
    }
  }
}