pipeline {
    agent any
    stages {
        stage('Submit Stack') {
            steps {
            sh "aws cloudformation create-stack --stack-name ec2 instance --template-body file://Cloudformation.yml --region 'ap-south-1b'"
              }
             }
            }
           }
