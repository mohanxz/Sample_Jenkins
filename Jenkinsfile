pipeline{
    agent any
        tools{
            jdk 'JDK 21'
            maven 'Maven 3'
        }
        stages{
            stage('Build Maven'){
                steps{
                    checkout scmGit(branches: [[name: '*/main']], extensions: [], userRemoteConfigs: [[url: 'https://github.com/mohanxz/Sample_Jenkins.git']])
                    bat 'mvn clean install'
                }
            }
           
        }
}