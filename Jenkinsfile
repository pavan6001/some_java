node {
   def anthome = tool name: 'ANT', type: 'ant' + '/bin/ant'
	stage('SCM Checkout') {
	   git branch: 'master',
	   credentialsId: 'Github credentials',
    	   url: 'https://github.com/pavan6001/some_java.git'
	 }
	
	stage('Ant Build') {
		sh "${ant} clean build compile jar"
	}
}
