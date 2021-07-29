properties([ disableConcurrentBuilds(), pipelineTriggers([githubPush()]) ]) 
 
node{
      deleteDir()
      checkout scm

     stage('deploying stack'){

      sh 'ansible-playbook cloudformation.yml -vvv'
      } 
     
}
