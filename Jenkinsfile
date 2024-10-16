pipeline {
    agent any
    stages {
        stage('Build Project') {
         steps {
              bat 'dotnet build'
            }
        }
        stage('Execute test') {
            stage ('Run npm audit tests') {
                steps {
                    bat 'dotnet test'
                    }
                }
        }   
    }   
}