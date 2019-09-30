pipeline {
    agent any 
    stages {
        stage('Build') {
          steps {
              echo 'Running build automation'
              sh 'ant clean '
              sh 'ant jar'
              archiveArtifacts artifacts: 'target/*.jar'
              }
            }
          }
         }
         
