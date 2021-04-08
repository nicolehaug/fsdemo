pipeline {
    agent any
    stages {
        stage('Provision Infrastructure') {
            steps {            

        sh '''

        cd home/nicole/fsdemo
           terraform refresh 
           terraform init           
           terraform plan -input=false
           terraform apply -auto-approve
           
           '''
                    
          } 
        }
      }
    }
