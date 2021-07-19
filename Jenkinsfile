pipeline {
   
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
    }
}
