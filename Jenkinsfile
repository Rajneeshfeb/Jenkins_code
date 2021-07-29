properties([ disableConcurrentBuilds(), pipelineTriggers([githubPush()]) ]) 
 
node{
      deleteDir()
      checkout scm

     stage('deploying stack'){

      sh 'ansible-playbook -c Cloudformation.yml'
      } 
     
}
