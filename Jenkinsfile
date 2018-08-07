pipeline {
  agent any
  stages {
    stage('first-solo') {
      steps {
        sh 'echo \'dummy text\''
      }
    }
    stage('parent') {
        parallel {
            stage('single-stage') {
              steps {
                sh 'echo \'dummy text\''
              }
            }
            
            stage('multiple-stages') {
                stages {
                    stage('first-sequential-stage') {
                      steps {
                        sh 'echo \'dummy text\''
                      }
                    }
                    stage('second-sequential-stage') {
                      steps {
                        sh 'echo \'dummy text\''
                      }
                    }
                    stage('third-sequential-stage') {
                      steps {
                        sh 'echo \'dummy text\''
                      }
                    }
                }
              post {
                success {
                  echo "This should show up in third-sequential-stage's list of steps"
                }
            }

            stage('other-single-stage') {
              steps {
                sh 'echo \'dummy text\''
              }
            }
        }
    }
    stage('second-solo') {
      steps {
        sh 'echo \'dummy text\''
      }
    }
  }
}
