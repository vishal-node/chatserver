pipeline {
  agent any
    
  tools {nodejs "NodeJs"}
    
  stages {
        
    stage('Git') {
      steps {
        git 'https://github.com/vishal-node/chatserver'
      }
    }
     
    stage('Build') {
      steps {
        sh 'npm install'
         sh '<<Build Command>>'
      }
    }  
    
            
    stage('Test') {
      steps {
        sh 'node test'
      }
    }
  }
}