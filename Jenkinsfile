#!groovy

node {
   
   step([$class: 'WsCleanup'])
   
   stages {
      
      stage "Checkout Git repo"
        checkout scm
      
      stage "postman_stage"
         steps {
            /* git 'https://github.com/SebastianUrbano/postman-newman-jenkins-github.git' **/
            sh 'npm install'
            sh 'npm run api-test-beforeproduction'
         }
  
   }
}
