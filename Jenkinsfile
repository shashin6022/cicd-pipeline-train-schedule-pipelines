pipeline {
  agent any
  stages {
    stage ('Build') {
      steps {
        echo "Running Build Automation"
        sh './gradlew build --no-deamon'
        archiveArtifacts artifacts: 'dist/trainSchedule.zip'
      }
    }
  }
}
