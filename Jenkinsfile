pipeline {
    agent any
    stages {
        stage('Provision Infrastructure') {
            steps {            

        sh '''
        
        sh script:'''
        
          dir("${env.WORKSPACE}/aQA"){
    sh "pwd"
}
         
           terraform init           
           terraform plan -input=false
           terraform apply -auto-approve
           
           '''
                    
          } 
        }
      }
    }
