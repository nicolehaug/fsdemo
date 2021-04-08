pipeline {
    agent any
          }
    stages {
        stage('Provision Infrastructure') {
            steps {
                script {
                
       def tfHome = tool name: 'TF_0.13.5'

        env.PATH = "${tfHome}:${env.PATH}"
        sh 'terraform -version'                

        sh '''

        cd fsdemo
           terraform refresh 
           terraform init           
           terraform plan -input=false
           terraform apply -auto-approve
           
           '''
                    
            } 
        }
    }
}
