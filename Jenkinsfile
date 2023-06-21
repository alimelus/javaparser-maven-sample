pipeline {
    agent any
     tools {
         maven 'MAVEN'
    }

    stages{
      stage("clone code")  {
            steps {
                script {
                    git 'https://github.com/alimelus/javaparser-maven-sample.git';
            }
            }
            }
        stage("mvn build") {
            steps {
                    sh 'mvn clean package'
         
                }
                }
            }
            }
