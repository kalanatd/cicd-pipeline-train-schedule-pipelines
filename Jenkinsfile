pipeline {
  agent any 
  stages {
    stage ('build') {
      steps {
        echo "running build automation"
        sh './gradlew build --no-deamon'
        archiveArtifcats artifacts: 'dist/trainSchedule.zip'
      }
    }
  }

}
