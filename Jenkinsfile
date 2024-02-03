pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=bhunnytoon -Dsonar.organization=natee-bhunnytoon -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=cd8d87c9f3d2ac5895e930dec2d34fc94f59747b'
			}
        } 
  }
}
