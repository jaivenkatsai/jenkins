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
              sh 'echo ${SAMPLE_URL}'
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
