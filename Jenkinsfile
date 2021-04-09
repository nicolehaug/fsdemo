pipeline {
    agent any
    stages {
        
     stage('Provision Infrastructure') {
            steps {
                script {

        env.PATH = "${tfHome}:${env.PATH}"
        sh 'terraform -version'                

        sh '''
           #echo "Plan $BUILD_NUMBER"
           #terraform init
           #terraform plan -out Plan_$BUILD_NUMBER -input=false
           #terraform apply -input=false Plan_$BUILD_NUMBER    
         
           terraform init           
           terraform plan -input=false
           terraform apply -auto-approve
           
           '''
                    
          } 
        }
      }
    }
}
