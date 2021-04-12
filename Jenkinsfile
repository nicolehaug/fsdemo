pipeline {
    agent any
    stages {
        
     stage('Test Change Directory') {
            steps {
                 dir('fsdemo') {
   terraform init
   terraform plan
   terraform apply
}
            }              
          } 
        }
      }
