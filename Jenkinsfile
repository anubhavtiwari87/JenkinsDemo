pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                sh '''
				dotnet restore Jenkins/Jenkins/Jenkins.csproj
				dotnet build Jenkins/Jenkins/Jenkins.csproj
				'''
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}
