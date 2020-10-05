pipeline {
    agent any 
    tools {
	  ant 'ANT'
	}
stages { 
    stage('Build') {
          steps {
              echo 'Running build automation'
              
                    sh 'ant jar'
                   

              //archiveArtifacts artifacts: '*/*.jar'
              }
          }
     }
}
         
