pipeline {
  agent any
  stages {
    stage ('Build') {
      steps {
        echo 'Running build automation'
        sh './gradlew build --no-daemon' # a background process for speeding up the process
        archiveArtifacts artifacts: 'dist/trainSchedule.zip'
      }
    }
  }
  
}
