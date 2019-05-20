pipeline {
  agent any
  stages {
    stage ("build") {
      steps {
        echo 'build first pipeline started'
        sh './gradlew build --no-daemon'
        archiveArtifacts artifacts: 'dist/trainschedule.zip'
      }
    }
  }
}
