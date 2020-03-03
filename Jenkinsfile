node {
        stage('Checkout') {
            git url: 'https://github.com/kash19/soapapi.git',  branch: 'master'
            echo '****************CHECKOUT SUCCESSFUL****************'
        }
       

       
			
	stage('Build') {
		def mvn_version = 'Maven_Home'
		withEnv( ["PATH+MAVEN=${tool mvn_version}/bin"]) {
			sh 'mvn site'
			}
		}
}
