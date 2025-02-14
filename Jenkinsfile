pipeline {
    agent any
    stages {
        stage('Restore Dependencies') {
            steps {
                bat 'dotnet restore'
            }
        }
        stage('Build Project') {
            steps {
                bat 'dotnet build'
            }
        }
        stage('Run dotnet test') {
            steps {
                bat 'dotnet test --logger "trx;LogFileName=test-results.trx"'
            }
        }
    }
}
