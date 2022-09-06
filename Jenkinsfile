pipeline{
  agent any
  stages{
    stage ('Build'){
      steps{
        echo 'Build is running'
        sh './gradlew build'
        archiveArtifacts artifacts: 'dist/trainSchedule.zip'
      }
    }
  }
}
