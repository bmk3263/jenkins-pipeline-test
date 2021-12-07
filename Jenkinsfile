pipeline{
    agent any 
   
    stages{
        stage('clone'){
         steps{
             git 'https://github.com/jabedhasan21/java-hello-world-with-maven.git'
         }   
        }
    stage('build-jenkins-2-branch'){
         steps{
          // first repository
    checkout([$class: 'GitSCM', branches: [[name: '*/jenkins-2']], doGenerateSubmoduleConfigurations: false, extensions: [[$class: 'RelativeTargetDirectory', relativeTargetDir: 'subdirectory1']], submoduleCfg: [], userRemoteConfigs: [[url: 'https://github.com/bmk3263/jenkins-pipeline-test.git']]])
load 'subdirectory1/Jenkinsfile'
         }   
        }




stage('build-jenkins-3-branch'){
         steps{
          // second repository
    checkout([$class: 'GitSCM', branches: [[name: '*/jenkins-3']], doGenerateSubmoduleConfigurations: false, extensions: [[$class: 'RelativeTargetDirectory', relativeTargetDir: 'subdirectory2']], submoduleCfg: [], userRemoteConfigs: [[url: 'https://github.com/bmk3263/jenkins-pipeline-test.git']]])
load 'subdirectory2/Jenkinsfile'
         }
        }       }
}
