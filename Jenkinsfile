pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=asgbuggywebapp123456 -Dsonar.organization=asgbuggywebapp123456 -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=744ac67afe5e72c747889e3f705a4c76e5d4924c'
			}
        } 
  }
}
