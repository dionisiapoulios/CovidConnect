pipeline {
  agent any
    
  tools {nodejs "NodeJS-16"}
    
  stages {
        
    stage('Git') {
      steps {
        git 'https://github.com/gfdb/soen390/tree/pipeline-testing'
      }
    }
     
    stage('Build') {
      steps {
        sh 'npm install'
      }
    }  
    
            
    stage('Test') {
      steps {
        sh 'node test'
      }
    }
  }
}
