pipeline {
  agent any
     tools { 
        maven 'MAVEN' 
        }
    stages{
        stage("mvn build") {
            steps {
                    sh 'mvn --debug clean package'
         
                }
                }
       stage('Docker Build and Tag') {
           steps {               
                sh 'docker build .' 
                //  sh 'docker tag nginxtest sunku/nginxtest:latest'
                // sh 'docker tag nginxtest sunku/nginxtest:$BUILD_NUMBER'
               
          }
        
            }
            }
