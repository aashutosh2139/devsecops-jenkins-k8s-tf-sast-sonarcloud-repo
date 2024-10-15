pipeline {
  agent any
  tools { 
        maven 'Maven_3_2_5'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=assgbuggywebapp_assgbuggywebapp -Dsonar.organization=assgbuggywebapp -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=c1cf9567662fefb82eec9d4f8a9f4e422f7cd153'
			}
        } 
  }
}
