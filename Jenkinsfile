pipeline{
  agent any
  stages{
    stage ('Build'){
      steps{
        echo 'Build is running'
        gradle wrapper
        sh './gradlew build --no-daemon --stacktrace'
        archiveArtifacts artifacts: 'dist/trainSchedule.zip'
      }
    }
  }
}
