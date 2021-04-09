pipeline {
    agent any
    stages {
        
     stage('Provision Infrastructure') {
            steps {
                             

        sh
         
         dir('/home/nicole/fsdemo') {
    // some block
}
           terraform init           
           terraform plan -input=false
           terraform apply -auto-approve
           
           
                    
          } 
        }
    }
}
