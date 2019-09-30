pipeline {
    agent any 
    stages {
        stage('Build') {
          steps {
              echo 'Running build automation'
              withAnt(installation: 'Ant') {
                    sh "ant jar"
                    }

              archiveArtifacts artifacts: '*/*.jar'
              }
            }
          }
         }
         
