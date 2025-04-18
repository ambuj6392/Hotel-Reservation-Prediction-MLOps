pipeline{
    agent any
    stages{
        stage('cloning github repo to jenkins'){
            steps{
                script{
                    echo 'cloning github repo to jenkins........'
                    checkout scmGit(branches: [[name: '*/main']], extensions: [], userRemoteConfigs: [[credentialsId: 'github-token', url: 'https://github.com/ambuj6392/Hotel-Reservation-Prediction-MLOps.git']])
                }
            }
        }
    }
}