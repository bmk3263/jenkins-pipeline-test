pipeline{
    agent any 
   parameters {
    gitParameter (branchFilter: 'origin/(.*)', defaultValue: 'master', name: 'BRANCH', type: 'PT_BRANCH')
  }
    stages{
        stage('clone'){
                     
         steps{
               echo "${params.branchFilter}"
         }

         }
        
        
      }
}
