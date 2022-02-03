pipeline{
    agent none
       agent {
           node{
               lable 'WORKSTATION'
           }
       }
    stages{
          
      stage('one') {
          steps {
              sh 'echo Hello World'
          }
          
        }
      stage('Two') {
          steps {
              sh 'echo Hello world'
          }
      }
    } 
}
