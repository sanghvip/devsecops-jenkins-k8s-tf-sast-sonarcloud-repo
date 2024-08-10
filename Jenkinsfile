pipeline {
  agent any
  tools { 
        maven 'Maven_3_2_5'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=devsecopsbuggywebapppratik -Dsonar.organization=devsecopsbuggywebapppratik -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=2c50bca15c049fb6965c22393fd7c123a0bb2d75'
			}
        } 
  }
}
