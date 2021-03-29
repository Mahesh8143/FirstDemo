pipeline {
    agent any
    
    environment{
        PATH= "C:/Soft/apache-maven-3.6.3/bin"
    }    
    stages{
        stage("CheckOut") {
            steps{
                checkout([$class: 'GitSCM', branches: [[name: '*/main']], extensions: [], userRemoteConfigs: [[url: 'https://github.com/Mahesh8143/FirstDemo.git']]])
            }
        }
        stage("Maven Build") {
           agent {
                docker { image 'node:14-alpine' }
            }
            steps {
                sh 'node --version'
            }
        }
    }
}
