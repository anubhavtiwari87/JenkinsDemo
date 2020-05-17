pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                sh '''
				dotnet restore Jenkins/Jenkins/optum.aru.fct.agent.csproj
				dotnet build Jenkins/Jenkins/optum.aru.fct.agent.csproj
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
