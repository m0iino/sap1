pipeline {
  agent any
    
  tools {nodejs "node12"}
    
  stages {
        
    stage('Cloning Git') {
      steps {
        git 'https://github.com/m0iino/sap1.git'
      }
    }
        
    stage('Install dependencies') {
      steps {
        sh 'npm install'
      }
    }
     
    stage('Test') {
      steps {
         sh 'npm test'
      }
    }      
  }
}
