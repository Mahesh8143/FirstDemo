
pipeline {
  agent any
 
  tools {
  maven 'Maven'
  }
  
  stages {
    
    stage ('Build') {
      
      steps {
      sh 'mvn clean install -f junit4-main/pom.xml'
      }
      
    } 
  }   
}  
