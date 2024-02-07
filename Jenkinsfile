pipeline {
  agent any
  tools { 
        maven 'Maven_3_2_5'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=bhunnytoon -Dsonar.organization=bhunnytoon -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=f4709f9a909040e963a9cdbe9fee3b10c038cc7a'
			}
        } 
  }
}
