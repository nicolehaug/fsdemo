pipeline {
    agent any
    stages {
        stage('Provision Infrastructure') {
            steps {            

        sh '''
        
        sh script:'''
          #!/bin/bash
          cd ./fsdemo
         
           terraform init           
           terraform plan -input=false
           terraform apply -auto-approve
           
           '''
                    
          } 
        }
      }
    }
