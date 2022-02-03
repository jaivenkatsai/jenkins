pipeline{
    agent none
//       agent {
//          node{
//              label 'WORKSTATION'
//           }
//     }
    stages {

        stage('one') {
            agent {
                node {
                  label 'NODEJS'
              }
          }
            steps {
              sh 'echo Hello World'
          }
          
        }
        stage('Two') {
            agent {
                node {
                    label 'JAVA'
                }
            }
          steps {
              sh 'echo Hello world'
          }
      }
    } 
}
