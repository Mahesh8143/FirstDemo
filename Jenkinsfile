pipeline {
    agent any
     
  
    stages{
        stage("CheckOut") {
            steps{
                checkout([$class: 'GitSCM', branches: [[name: '*/main']], extensions: [], userRemoteConfigs: [[url: 'https://github.com/Mahesh8143/FirstDemo.git']]])
            }
        }
        stage("Maven Build") {
            steps {
                sh  'mvn validate'
            }
        }
    }
}
