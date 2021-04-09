pipeline {
    agent any
    stages {
        
     stage('Provision Infrastructure') {
            steps {
                script {               

        sh ''' 
         
           terraform init           
           terraform plan -input=false
           terraform apply -auto-approve
           
           '''
                    
          } 
        }
      }
    }
}
