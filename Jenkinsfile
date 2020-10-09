pipeline {
    agent any 
stages { 
    stage('Build') {
          steps {
              echo 'Running build automation'
              def anthome = tool name: 'ANT', type: 'ant'
		  sh "${anyhome}/bin clean compile jar run"
                   

              //archiveArtifacts artifacts: '*/*.jar'
              }
          }
     }
}
         
