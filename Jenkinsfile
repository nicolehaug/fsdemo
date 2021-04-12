pipeline {
    agent any
    stages {
        
     stage('Change working directory...') {
            agent { docker 'my-image' }

            steps {
                dir('fsdemo') {
                    sh 'pwd'
                }
            }              
          } 
        }
      }
