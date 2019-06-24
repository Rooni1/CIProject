pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh 'echo Build'
       
      }
    }
    stage('Performance Test') {
      parallel {
        stage('Performance Test') {
          steps {
            sh 'echo Performance Test'
            
          }
        }
        stage('Unit Test') {
          steps {
            sh 'echo Unit Test'
          }
        }
      }
    }
    stage('Static Analysis') {
      steps {
        sh 'echo Static Analysis'
      }
    }
    stage('Deploy') {
      steps {
        sh 'echo Deploy'
      }
    }
  }
}