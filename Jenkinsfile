pipeline{
  agent any
  stages{
    stage ('Build'){
      steps{
        echo 'Build is running'
        sh './gradlew build --no-daemon'
        archiveArtifacts artifacts: 'dist/trainSchedule.zip'
        sh './gradlew npm_start'
      }
    }
  }
}
