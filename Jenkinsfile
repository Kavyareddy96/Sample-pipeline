pipeline {
    agent { label 'Agent_Mvn_01' }
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
                sh 'git clone https://github.com/Kavyareddy96/Sample-pipeline.git'
				
            }
        }
        stage('Build') {
            steps {
                sh 'mvn clean install'
			
            }
        }
       
    }
}
