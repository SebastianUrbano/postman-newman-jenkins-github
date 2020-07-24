#!groovy

node {
   
   step([$class: 'WsCleanup'])
   
   stage "Checkout Git repo"
      checkout scm
      
   stage "postman_stage"
      /* git 'https://github.com/SebastianUrbano/postman-newman-jenkins-github.git' **/      
      sh 'npm install'
      sh 'npm run api-test-beforeproduction'
}
