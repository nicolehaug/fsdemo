pipeline {
    agent any
    stages {
        
     stage('Test Change Directory') {
            steps {
                bash 'cd fsdemo'
                bash 'ls -la'
                bash 'echo $PATH'
            }
        
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
}
