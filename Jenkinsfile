pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=thinkingmonster_thinkingmonster -Dsonar.organization=thinkingmonster -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=f7c449c73cb300ab34bdfcce38332d04fde2558c'
			}
        } 
  }
}
