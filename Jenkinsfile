pipeline{
  agent any
  stages{
    stage ('Build'){
      steps{
        echo 'Build is running'
        sh './gradlew build --no-daemon --stacktrace'
        archiveArtifacts artifacts: 'dist/trainSchedule.zip'
      }
    }
  }
}
