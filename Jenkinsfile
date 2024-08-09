pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=testbuggywebtoken -Dsonar.organization=Jenkins-Test-buggyapp -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=4cc8379df0f222433242858faa96698eff5e6277'			}
        } 
  }
}
