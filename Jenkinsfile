pipeline{
    agent none
//       agent {
//          node{
//              label 'WORKSTATION'
//           }
//     }
    ptions{.disableConcurrentBuilds()  }
    environment {
        SAMPLE_URL = 'google.com'
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
        environment {
            SAMPLE_URL = 'yahoo.com'
        }
          steps {
              sh 'echo Hello world'
              sh 'echo ${SAMPLE_URL}'
          }
      }
    }
}
