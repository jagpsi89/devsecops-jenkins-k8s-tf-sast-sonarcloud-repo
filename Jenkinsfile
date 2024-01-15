pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=jaggibuggywebapp -Dsonar.organization=jaggibuggywebapp -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=537ef5d69358afdb3de284581df576177fbabfb5'
			}
        } 
  }
}
