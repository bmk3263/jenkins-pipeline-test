pipeline{
    agent any 
   parameters {
    
       string(name: "TEST_STRING", defaultValue: "ssbostan", trim: true, description: "Sample string parameter")
  }
    stages{
        stage('clone'){
                     
         steps{
               echo "${params.TEST_STRING}"
         }

         }
        
        
      }
}
