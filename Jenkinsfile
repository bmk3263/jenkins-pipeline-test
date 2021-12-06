pipeline{
    agent any 
   
    stages{
        stage('clone'){
         steps{
             git 'https://github.com/jabedhasan21/java-hello-world-with-maven.git'
         }   
        }
    stage('build'){
         steps{
            sh 'mvn clean install'
         }   
        }
        }
}
