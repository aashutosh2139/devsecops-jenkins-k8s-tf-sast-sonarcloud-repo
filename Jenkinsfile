pipeline {
  agent any
  tools { 
        maven 'Maven_3_2_5'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=asgbuggywebsap_asgbuggywebsap -Dsonar.organization=asgbuggywebsap -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=09158b30933fa5b2642654b60bc8e136e0ceffb4'
			}
        } 
  }
}
