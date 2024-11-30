pipeline {
  agent any
  tools { 
        maven 'Maven_3_2_5'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=asgbuggywebapp-test_jb-devsecops-test -Dsonar.organization=jb-devsecops-test -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=9d775f336a342253461b3b638b1639f11f1a94bb'
			}
        } 
  }
}
