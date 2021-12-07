pipeline{
    agent any 
   
    stages{
        stage('clone'){
                     
         steps{
               git url: https://github.com/bmk3263/jenkins-pipeline-test.git
               def v = version()
                   if (v) {
                       echo "Building version ${v}"   
                   }

         }
        }       }
}
