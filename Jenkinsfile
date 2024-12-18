pipeline{
    agent any
    tools{
        nodejs 'Node Js'
    }
    options{
        timeout(time: 300, unit: 'SECONDS')
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