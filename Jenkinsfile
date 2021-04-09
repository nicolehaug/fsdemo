pipeline {
    agent any
    stages {
        
     stage('Provision Infrastructure') {
            steps {
                script {            

        sh '''
         
         dir('/home/nicole/fsdemo') {
    // some block
}
           terraform init           
           terraform plan 
           terraform apply -auto-approve
           
           '''
                    
          } 
        }
    }
}
}
