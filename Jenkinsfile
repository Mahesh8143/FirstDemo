
pipeline {
  agent any
  
  stages {
    
    stage ('Build') {
      
       steps {
        withSonarQubeEnv('SonarQube') {
        sh 'mvn -f junit4-main/pom.xml sonar:sonar'
       }
      
    } 
  }   
}  
