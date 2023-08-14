pipeline {
    agent any
    stages {
        stage('Example Build') {
            steps {
                echo 'Hello World'
            }
        }
        stage('Deploy') {
            when {
                branch 'production'
            }
                steps {
                    echo 'Deploying main branch'
                }    
        }
    }
}
