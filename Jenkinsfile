pipeline {
   environment {
    registry = "jessiegift/scacloud"
    registryCredential = 'Docker'
    dockerImage = ''
  }
    agent any
     tools {nodejs "nodejs"}
    stages {
       stage('Cloning Git') {
      steps {
        git 'https://github.com/jessiegift/SCA-CLOUD-SCHOOL-APPLICATION.git'
      }
    }
 stage('Build') { 
            steps {
                sh 'npm install' 
            }
        }
      
         stage('Building image') {
      steps{
        script {
          dockerImage = docker.build registry + ":$BUILD_NUMBER"
        }
      }
    }
    stage('Deploy Image') {
      steps{
        script {
          docker.withRegistry( '', registryCredential ) {
            dockerImage.push()
          }
        }
      }
    }
    }
