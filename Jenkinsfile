@Library('my-shared-library@master','my-shared-library2@main')_

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
