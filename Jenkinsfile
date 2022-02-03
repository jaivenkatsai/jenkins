pipeline{
    agent none
//       agent {
//          node{
//              label 'WORKSTATION'
//           }
//     }

    environment {
        SAMPLE_URL = 'GOOGLE.COM'
    }
    stages {

        stage('one') {
            agent {
                node {
                  label 'NODEJS'
              }
          }
            steps {
              sh 'echo Hello World'
              sh .
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
