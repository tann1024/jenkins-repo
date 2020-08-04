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
                            steps {
                                    input('Do you want to proceed with UAT?')
			    }
		    }
                    stage('Four') {
                            steps {
                                    input('Do you want to proceed with PROD?')
			    }
                    }
                    stage('Five') {
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
