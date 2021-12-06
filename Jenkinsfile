pipeline{
    agent any 
   
    stages{
        stage('clone'){
         steps{
             git 'https://github.com/jabedhasan21/java-hello-world-with-maven.git'
         }   
        }
    stage('input'){
         steps{
            input('do you want proceed?')
         }   
        }
        }
}
