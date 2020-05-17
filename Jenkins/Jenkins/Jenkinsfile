pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                sh '''
				dotnet restore optum.aru.fct.agent.csproj
				dotnet build optum.aru.fct.agent.csproj
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