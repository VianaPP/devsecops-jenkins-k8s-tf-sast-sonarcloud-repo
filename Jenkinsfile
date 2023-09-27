pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=secopsbugwebapp -Dsonar.organization=secopsbugwebapp -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=5c42a4161dd3d37ada0efdd67ad3e48567c2f9b1'
			}
        } 
  }
}
