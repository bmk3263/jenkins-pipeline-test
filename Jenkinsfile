pipeline{
    agent any 
   parameters {
    gitParameter branchFilter: 'origin/(.*)', defaultValue: 'master', name: 'BRANCH', type: 'PT_BRANCH'
  }
    stages{
        stage('clone'){
                     
         steps{
               git branch: "${params.BRANCH}", url:  'https://github.com/bmk3263/jenkins-pipeline-test.git'
               def v = version()
                   if (v) {
                       echo "Building version ${v}"   
                   }
         }

         }
        
        
      }
}
