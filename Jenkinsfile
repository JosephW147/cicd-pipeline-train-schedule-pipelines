pipeline{
  agent any
  stages{
    stage('Build'){
      steps{
        echo 'Running building automation'
          sh './gradlew build --no daemon'
          archiveArtifacts artifacts: 'dist/trainSchedule.zip'
      }
    }      
  }
}
