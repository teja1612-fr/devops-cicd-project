pipeline {
    agent any

    stages {
        
		
		stage('Build Artifact ') {
            steps {
                echo 'generating artifact with maven build tool'
				sh 'mvn clean install'
            }
        }
		
		
    }
}
