pipeline {
    agent { label 'Agent_mvn_01' }
    stages {
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
