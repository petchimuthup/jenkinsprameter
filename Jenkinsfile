pipeline {
    agent any
    stages {
        stage('Example Build') {
            steps {
                echo 'Hello World'
            }
        }
        stage('Example Deploy') {
            when {
                branch 'production'
                }
            parallel {
                stage('deploy production branch') {
                    steps {
                        echo 'Deploying production'
                    }
                }
            }
            stage('verify') {
               steps {
                   echo 'welcome'
               }
            
            }
        }
    }
}
