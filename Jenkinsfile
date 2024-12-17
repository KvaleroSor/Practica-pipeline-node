pipeline{
    agent any
    tools{
        nodejs 'nodejs'
    }

    stages{
        stage('Instal·lant dependències'){
            steps{
                sh 'npm install'
            }
        }
        stage('Corrent linter'){
            steps{
                sh 'npm run lint'
            }
        }
        stage('Corrent jest'){
            steps{
                sh 'npm run test'
            }
        }
        stage('Desplegant'){
            steps{
                sh 'npm start'
            }
        }
    }
}