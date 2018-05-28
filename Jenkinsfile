pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh 'mvn clean source:jar package'
        input 'This is a very long message to simulate a very long message, this is a very long message to simulate a very long message.'
      }
    }
    stage('Browser Tests') {
      parallel {
        stage('Firefox') {
          steps {
            sh 'echo \'setting up selenium environment\''
            sh 'ping -c 5 localhost'
          }
        }
        stage('Safari') {
          steps {
            sh 'echo \'setting up selenium environment\''
            sh 'ping -c 8 localhost'
          }
        }
        stage('Chrome') {
          steps {
            sh 'echo \'setting up selenium environment\''
            sh 'ping -c 3 localhost'
          }
        }
        stage('Internet Explorer') {
          steps {
            sh 'echo \'setting up selenium environment\''
            sh 'ping -c 4 localhost'
          }
        }
        stage('Firefox1') {
          steps {
            sh 'echo \'setting up selenium environment\''
            sh 'ping -c 5 localhost'
          }
        }
        stage('Safari1') {
          steps {
            sh 'echo \'setting up selenium environment\''
            sh 'ping -c 8 localhost'
          }
        }
        stage('Chrome1') {
          steps {
            sh 'echo \'setting up selenium environment\''
            sh 'ping -c 3 localhost'
          }
        }
        stage('Internet Explorer1') {
          steps {
            sh 'echo \'setting up selenium environment\''
            sh 'ping -c 4 localhost'
          }
        }
        stage('Firefox2') {
          steps {
            sh 'echo \'setting up selenium environment\''
            sh 'ping -c 5 localhost'
          }
        }
        stage('Safari2') {
          steps {
            sh 'echo \'setting up selenium environment\''
            sh 'ping -c 8 localhost'
          }
        }
        stage('Chrome2') {
          steps {
            sh 'echo \'setting up selenium environment\''
            sh 'ping -c 3 localhost'
          }
        }
        stage('Internet Explorer2') {
          steps {
            sh 'echo \'setting up selenium environment\''
            sh 'ping -c 4 localhost'
          }
        }
        stage('Firefox3') {
          steps {
            sh 'echo \'setting up selenium environment\''
            sh 'ping -c 5 localhost'
          }
        }
        stage('Safari3') {
          steps {
            sh 'echo \'setting up selenium environment\''
            sh 'ping -c 8 localhost'
          }
        }
        stage('Chrome3') {
          steps {
            sh 'echo \'setting up selenium environment\''
            sh 'ping -c 3 localhost'
          }
        }
        stage('Internet Explorer3') {
          steps {
            sh 'echo \'setting up selenium environment\''
            sh 'ping -c 4 localhost'
          }
        }
        stage('Firefox4') {
          steps {
            sh 'echo \'setting up selenium environment\''
            sh 'ping -c 5 localhost'
          }
        }
        stage('Safari4') {
          steps {
            sh 'echo \'setting up selenium environment\''
            sh 'ping -c 8 localhost'
          }
        }
        stage('Chrome4') {
          steps {
            sh 'echo \'setting up selenium environment\''
            sh 'ping -c 3 localhost'
          }
        }
        stage('Internet Explorer4') {
          steps {
            sh 'echo \'setting up selenium environment\''
            sh 'ping -c 4 localhost'
          }
        }
        stage('Firefox5') {
          steps {
            sh 'echo \'setting up selenium environment\''
            sh 'ping -c 5 localhost'
          }
        }
        stage('Safari5') {
          steps {
            sh 'echo \'setting up selenium environment\''
            sh 'ping -c 8 localhost'
          }
        }
        stage('Chrome5') {
          steps {
            sh 'echo \'setting up selenium environment\''
            sh 'ping -c 3 localhost'
          }
        }
        stage('Internet Explorer5') {
          steps {
            sh 'echo \'setting up selenium environment\''
            sh 'ping -c 4 localhost'
          }
        }
        stage('Firefox6') {
          steps {
            sh 'echo \'setting up selenium environment\''
            sh 'ping -c 5 localhost'
          }
        }
        stage('Safari6') {
          steps {
            sh 'echo \'setting up selenium environment\''
            sh 'ping -c 8 localhost'
          }
        }
        stage('Chrome6') {
          steps {
            sh 'echo \'setting up selenium environment\''
            sh 'ping -c 3 localhost'
          }
        }
        stage('Internet Explorer6') {
          steps {
            sh 'echo \'setting up selenium environment\''
            sh 'ping -c 4 localhost'
          }
        }
        stage('Firefox7') {
          steps {
            sh 'echo \'setting up selenium environment\''
            sh 'ping -c 5 localhost'
          }
        }
        stage('Safari7') {
          steps {
            sh 'echo \'setting up selenium environment\''
            sh 'ping -c 8 localhost'
          }
        }
        stage('Chrome7') {
          steps {
            sh 'echo \'setting up selenium environment\''
            sh 'ping -c 3 localhost'
          }
        }
        stage('Internet Explorer7') {
          steps {
            sh 'echo \'setting up selenium environment\''
            sh 'ping -c 4 localhost'
          }
        }
        stage('Firefox8') {
          steps {
            sh 'echo \'setting up selenium environment\''
            sh 'ping -c 5 localhost'
          }
        }
        stage('Safari8') {
          steps {
            sh 'echo \'setting up selenium environment\''
            sh 'ping -c 8 localhost'
          }
        }
        stage('Chrome8') {
          steps {
            sh 'echo \'setting up selenium environment\''
            sh 'ping -c 3 localhost'
          }
        }
        stage('Internet Explorer8') {
          steps {
            sh 'echo \'setting up selenium environment\''
            sh 'ping -c 4 localhost'
          }
        }
        stage('Firefox9') {
          steps {
            sh 'echo \'setting up selenium environment\''
            sh 'ping -c 5 localhost'
          }
        }
        stage('Safari9') {
          steps {
            sh 'echo \'setting up selenium environment\''
            sh 'ping -c 8 localhost'
          }
        }
        stage('Chrome9') {
          steps {
            sh 'echo \'setting up selenium environment\''
            sh 'ping -c 3 localhost'
          }
        }
        stage('Internet Explorer9') {
          steps {
            sh 'echo \'setting up selenium environment\''
            sh 'ping -c 4 localhost'
          }
        }
      }
    }
    stage('Static Analysis') {
      steps {
        sh 'mvn findbugs:findbugs'
      }
    }
    stage('Deploy') {
      parallel {
        stage('Deploy') {
          steps {
            sh 'mvn source:jar package -Dmaven.test.skip'
          }
        }
        stage('final') {
          steps {
            echo 'fdsf223'
          }
        }
      }
    }
  }
  post {
    always {
      junit '**/target/surefire-reports/TEST-*.xml'
      archive '**/target/*.jar'

    }

  }
}