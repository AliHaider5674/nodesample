@Library('my-shared-library')_
#!/usr/bin/env groovy

pipeline {

    agent {
        docker {
            image 'node'
            args '-u root'
        }
    }

    stages {
        stage('Build') {
            steps {
                script {
                    echo 'Building...'
                    commonFunctions 
                    
                }
            }
        }
    }
}
