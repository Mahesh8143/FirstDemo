pipeline {
    agent any
     
    environment {
        PATH = "C:/Soft/apache-maven-3.6.3"
        Path = "c:/windows/system32"
    }
    
    stages{
        stage("CheckOut") {
            steps{
                checkout([$class: 'GitSCM', branches: [[name: '*/main']], extensions: [], userRemoteConfigs: [[url: 'https://github.com/Mahesh8143/FirstDemo.git']]])
            }
        }
        stage("Maven Build") {
            steps {
                bat 'cd C:/Soft'
            }
        }
    }
}
