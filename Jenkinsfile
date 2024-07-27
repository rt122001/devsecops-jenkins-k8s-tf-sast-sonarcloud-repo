pipeline {
  agent any
  tools { 
        maven 'Maven_3_2_5'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=asgbuggywebapp22b -Dsonar.organization=asgbuggywebapp22b -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=a15e039eff6db3340c47a59f1cd989e81f372ffa'
			}
        } 
  }
}
