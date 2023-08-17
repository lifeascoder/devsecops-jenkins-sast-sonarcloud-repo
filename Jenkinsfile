pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=adityabuggyapp -Dsonar.organization=adityabuggyapp -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=1fb962ab19db85eeb446cbd408577371bbf1694f'
			}
        } 
  }
}
