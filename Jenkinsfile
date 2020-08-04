pipeline {
    agent any
            stages {
                    stage('One') {
                            steps {
                                    echo 'This is a Demo project'
                            }
                    }
                
                    stage('Two') {
                            steps {
                                    input('Do you want to proceed with DEV?')
                            }
                    }
                    stage('Three') {
                        when {
                            not {
                                  branch "master"
                            }
                        }
                        steps {
                                echo "Done with deployment"
                        }
                    }
                 }
            }
