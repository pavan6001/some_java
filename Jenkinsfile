pipeline {
    agent any 
    stages {
        stage('Build') {
          steps {
              echo 'Running build automation'
              withAnt(installation: 'Ant') {
                    ant jar
                    }

              archiveArtifacts artifacts: 'target/*.jar'
              }
            }
          }
         }
         
