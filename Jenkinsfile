pipeline {
  agent any
  stages {
    stage ('Build') {
      steps{
        echo 'Running gradle build'
        sh './gradlew build --no-daemon'
        archiveArtifcts artifacts: 'dist/trainSchedule.zip'
      }
    }
  }
}
