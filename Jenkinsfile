pipeline{
    agent none
      agent {
         node {
             lable 'WORKSTATION'
         }
      } 
      stages('one') {
          agent {
              
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
