pipeline{
    agent none
       agent {
           node{
               lable 'WORKSTATION'
           }
       }
    stages{
          
      stage('one') {
          agent {
              node {
                  
              }
          }
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
