pipeline {
  agent any
  stages {
    stage ('Build') {
      steps {
        echo 'Running build automation'
        sh './gradlew build --no-daemon'
        archiveArtifacts artifacts: 'dist/trainSchedule.zip'
        sh 'echo "Hello World"'
         sh '''
             echo "Multiline shell steps works too"
             ls -lah
         '''
      }
    }
  }
}
