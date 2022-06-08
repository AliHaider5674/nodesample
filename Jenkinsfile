@Library('my-shared-library')_
@Library('my-shared-library2')

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
                    commonFunctions 'ali'
                    sample 
                }
            }
        }
    }
}
