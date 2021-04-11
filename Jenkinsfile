pipeline {
    agent any
    stages {
        
     stage('Provision Infrastructure') {
            steps {
                script {            

   sh 'cd fsdemo'
           terraform init           
           terraform plan 
           terraform apply -auto-approve
           
           
                    
          } 
        }
    }
}
}
