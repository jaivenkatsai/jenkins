pipeline{
    agent none
//       agent {
//          node{
//              label 'WORKSTATION'
//           }
//     }
    options { disableConcurrentBuilds() }

    parameters {
        string(name: 'PERSON', defaultValue: 'Mr Jenkins', description: 'Who should i say hello to?')

        text(name: BIOGRAPHY, defaultValue: '', description: 'Enter some information about the person')

        booleanParam(name: TOGGLE, defaultValue: true, description: 'Togle this Value')

        choice(name: 'CHOICE', choices: ['one', 'tow', 'three'], description: 'pick something')

        password(name: 'PASSWORD', defaultValue: 'SECRET', description: 'Enter a password')
    }
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
