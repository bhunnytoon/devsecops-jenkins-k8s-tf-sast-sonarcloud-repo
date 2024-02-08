pipeline {
  agent any
  tools { 
        maven 'Maven_3_2_5'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=bhunnytoon -Dsonar.organization=bhunnytoon -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=f478dceb39e2fb62ce2622216a3112a7186cb2e1'
			}
        } 
  }
}
