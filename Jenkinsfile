properties([ disableConcurrentBuilds(), pipelineTriggers([githubPush()]) ]) 

pipeline{
    agent any
    stages{
        stage('Submit Stack'){
            steps{
            sh "aws cloudformation create-stack --stack-name EC2Instance --template-body file://Cloudformation.yml --region ap-south-1"
            sh "aws cloudformation delete-stack stack_name EC2Instance"
              }
             }
            }
           }
