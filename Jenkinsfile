pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=devsecops876 -Dsonar.organization=devsecops -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=0ddfd1d73dc282f8d9db60eadd66110e180fe76d'
			}
        } 
  }
}
