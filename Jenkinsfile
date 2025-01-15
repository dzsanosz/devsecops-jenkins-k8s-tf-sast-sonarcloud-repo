pipeline {
  agent any
  tools { 
        maven 'Maven_3_2_5'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=dzsanosz-buggy-webapp -Dsonar.organization=dzsanosz-buggy-webapp -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=28f03d6170410a9699ca1a7585bebf128ac89c91'
			}
        } 
  }
}
