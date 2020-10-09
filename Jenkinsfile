node {
   	stage('SCM Checkout') {
	   git branch: 'master',
	   credentialsId: 'Github credentials',
    	   url: 'https://github.com/pavan6001/some_java.git'
	 }
	
	stage('Ant Build') {
		def antVersion = 'Ant1.10.5'
		withEnv( ["ANT_HOME=${tool antVersion}"] ) {
		sh "$ANT_HOME/bin/ant clean build compile jar"
		}
	}
}
