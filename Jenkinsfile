pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=natee-securityguru -Dsonar.organization=natee-securityguru -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=6a1187bc7577cd315ff682c540405c5ec144dfaa'
			}
        } 
  }
}
