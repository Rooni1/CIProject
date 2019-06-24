pipeline {
    agent any
    
    tools {nodejs "node"}

    stages {
         stage('dep') {
            steps {
                bat 'npm install'
            }
        }
        stage('builds') {
            steps {
                bat 'npm run build'
            }
        }
        stage('tests') {
            steps {
                bat 'npm run test'
            }
        }
        stage('deploys ') {
            steps {
                bat 'npm run deploy'
            }
        }
    }
}
