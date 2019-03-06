pipeline {
  agent any
  stages {
      stage('Build Docker images and push to ecr'){
          steps {
          sh 'docker build -f "dockerfile" -t docker/nginx:latest .'
          sh 'docker push aws_account_id.dkr.ecr.us-east-1.amazonaws.com/example/docker/nginx:latest'
          }
      }
   
    }
}
