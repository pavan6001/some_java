pipeline {
    agent any 
    stages {
        stage('Build') {
          steps {
              echo 'Running build automation'
              withAnt(installation: 'Ant') {
                    sh "ant build"
                    }

              archiveArtifacts artifacts: 'target/*.jar'
              }
            }
          }
         }
         
