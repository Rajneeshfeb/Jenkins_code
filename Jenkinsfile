properties([ disableConcurrentBuilds(), pipelineTriggers([githubPush()]) ]) 

pipeline{
    agent any
    stages{
        stage('Submit Stack'){
            steps{
            sh "aws cloudformation create-stack --stack-name EC2Instance --template-body Cloudformation.yml --region ap-south-1"
              }
             }
            }
           }
