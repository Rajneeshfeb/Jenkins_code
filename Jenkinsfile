properties([ disableConcurrentBuilds(), pipelineTriggers([githubPush()]) ]) 
 
node{
      deleteDir()
      checkout scm

     stage('deploying stack'){

      sh 'Cloudformation.yml'
      } 
     
}
