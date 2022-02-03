pipeline{
    agent none
      agent {
         node {
             lable 'WORKSTATION'
         }
      } 
    stages  {
         
        stage ('one') {
           agent {
               node {
                  lable 'NODEJS'
          }
          
        }
      stage('Two') {
          steps {
              sh 'echo Hello world'
          }
      }
    } 
}
