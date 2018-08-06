pipeline {
    agent any
    stages {
        stage("build and deploy") {
            parallel {
                stage("first") {
                    stages {
                        stage("build") {
                            steps {
                                sh 'echo \'dummy text\''
                            }
                        }
                        stage("deploy") {
                            steps {
                                sh 'echo \'dummy text\''
                            }
                        }
                    }
                }

                stage("second") {
                    stages {
                        stage("build") {
                            steps {
                                sh 'echo \'dummy text\''
                            }
                        }
                        stage("deploy") {
                             steps {
                                sh 'echo \'dummy text\''
                            }
                        }
                    }
                }
            }
        }
    }
}
