pipeline {
    agent any
    stages {
	    stage('Parallel Execution') {
		   parallel {
		    stage('Clean up') {
			   steps {
			      cleanWs()
				 }
			}
        stage('Clone') {
            steps {
                git branch: 'main', url: 'https://github.com/Kavyareddy96/java-war-repo.git'
				
            }
        }
        stage('Build') {
            steps {
                sh 'mvn clean install'
			
            }
        }
       
    }
}
