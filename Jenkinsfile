pipeline {
  agent any
  tools { 
        maven 'Maven_3.5.2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=dsi-test -Dsonar.organization=dsi-test -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=d1e471b1abf72ff2f2bb564800870a8b61396c6d'
			}
        } 
  }
}
