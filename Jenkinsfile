pipeline {
    agent any 
    tools {
	  ant 'ANT'
	}
    
    stage('Build') {
          steps {
              echo 'Running build automation'
              
                    sh "ant jar"
                   

              #archiveArtifacts artifacts: '*/*.jar'
              }
          }
}
        
         
