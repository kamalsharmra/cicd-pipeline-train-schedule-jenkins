pipeline {
  agent any
  stages {
    stage('Build') {
      echo 'Running gradle build'
      sh './gradlew build --no-daemon'
      archiveArtifcts artifacts: 'dist/trainSchedule.zip' 
    }
  }
}
