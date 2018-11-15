#!groovy

node {
	   
	stage('Checkout'){

          checkout scm
       }

       stage('BuildArtifact'){
	        def mvn_version = 'M3'
         withEnv( ["PATH+MAVEN=${tool mvn_version}/bin"] )
	       {

          sh 'mvn install'
	       }
       }
	   
      /*
	stage('Sonar') {
                    //add stage sonar
                    sh 'mvn sonar:sonar'
                }
		*/
       
}
