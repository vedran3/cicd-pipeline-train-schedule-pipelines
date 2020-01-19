pipeline {
  agent any
  stages {
    stage ('Build') {
      steps {
        echo 'Running build automation'
        sh './gradlew build --no-daemon'
        archiveArtifacts artifacts: 'dist/trainSchedule.zip'
    stage ('Echo') {
      steps {
        echo 'This is the 2nd step'
      }
        }  
      }
    }
  }
}
