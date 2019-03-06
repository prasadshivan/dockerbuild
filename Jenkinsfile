pipeline {
  agent any
  stages {
      stage('Build Docker images and push to ecr'){
          steps {
          sh 'docker build -f "dockerfile" -t nginx:latest 447895454160.dkr.ecr.us-east-1.amazonaws.com/example/nginx/nginx'
          sh 'docker push 447895454160.dkr.ecr.us-east-1.amazonaws.com/example/nginx/'
          }
      }
   
    }
}
