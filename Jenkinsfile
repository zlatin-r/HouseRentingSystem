pipeline {
    agent any
    stages {
        stage('Build project') {
            steps {
                bat 'dotnet build'
            }
        }
        stage('Run dotnet test') {
            steps {
                bat 'dotnet test'
            }
        }
    }
}
