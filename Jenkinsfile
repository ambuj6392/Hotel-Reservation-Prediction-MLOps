pipeline{
    agent any

    environment{
        VENV_DIR = 'venv'
    }


    stages{
        stage('cloning github repo to jenkins'){
            steps{
                script{
                    echo 'cloning github repo to jenkins........'
                    checkout scmGit(branches: [[name: '*/main']], extensions: [], userRemoteConfigs: [[credentialsId: 'github-token', url: 'https://github.com/ambuj6392/Hotel-Reservation-Prediction-MLOps.git']])
                }
            }
        }

        stage('Setting up our Virtual Environment and Installing dependancies'){
            steps{
                script{
                    echo 'Setting up our Virtual Environment and Installing dependancies............'
                    sh '''
                    python -m venv ${VENV_DIR}
                    . ${VENV_DIR}/bin/activate
                    pip install --upgrade pip
                    pip install -e .
                    '''
                }
            }
        }

    }
}