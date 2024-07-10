pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=toddbuggywebapptestv1 -Dsonar.organization=Jenkins-Test-buggyapp -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=bc99d821e75b7738ca1c3a37d0d5e069dbbccd67'
			}
        } 
  }
}
