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
                  lable 'NODEJS'
              }
          }
            steps {
              sh 'echo Hello World'
          }
          
        }
        stage('Two') {
            agent {
                node{}
            }
          steps {
              sh 'echo Hello world'
          }
      }
    } 
}
