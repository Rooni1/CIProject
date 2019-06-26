pipeline {
    agent any
    
    tools {nodejs "node"}

    stages {
         stage('Dependencies') {
            steps {
                bat 'npm install'
            }
        }
        stage('Builds') {
            steps {
                bat 'npm run build'
            }
        }
        stage('Tests') {
            steps {
                bat 'npm run test'
            }
        }
        stage('Deploys ') {
            steps {
                bat 'npm run deploy'
            }
        }
    }
}
