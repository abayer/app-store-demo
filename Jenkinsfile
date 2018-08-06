pipeline {
  agent any
  stages {
        stage("first stage") {
            stages {
               stage("build") {
                   steps {
                       sh 'echo \'dummy text\''
                   }
               }
               stage("test") {
                   steps {
                       sh 'echo \'dummy text\''
                   }
               }
            }
        }

        stage("second stage") {
            stages {
               stage("build") {
                   steps {
                       sh 'echo \'dummy text\''
                   }
               }
               stage("test") {
                   steps {
                       sh 'echo \'dummy text\''
                   }
               }
            }
        }
    }
}
