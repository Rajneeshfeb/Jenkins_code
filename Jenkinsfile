properties([ disableConcurrentBuilds(), pipelineTriggers([githubPush()]) ]) 

pipeline{
    agent any
    stages{
        stage('Submit Stack'){
            steps{
            sh "aws cloudformation update-stack --stack-name EC2Instance --template-body file://Cloudformation.yml --region ap-south-1"
              }
             }
            }
           }
