pipeline {
  agent any
  stages { 
   stages ('Build'){
     stages {
       echo 'Running build automation'
       sh './gradlew build --no-daemon'
       archiveArtifacts artifacts: 'dist/trainSchedule.zip'
     }
   }
  }
}
