pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=devsecopsproj -Dsonar.organization=devsecopsproj -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=5c998f5f3ed54c293d20e1387e8c8a57f8a604c8
			}
        } 
  }
}
